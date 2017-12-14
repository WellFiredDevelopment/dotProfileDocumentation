Processors
==========

Introduction
------------

A processor facilitates .Profiles processing of data, if probes extract data, processors process them into a usable
format. .Profile comes with a selection of processors built in, allowing you to get up and running with little to no
effort.

think of probes as the input and processors as the output, with a .Profile sessions sitting in the middle, controlling
the whole thing.

Provided Processors
-------------------

.Profile provides a selection of processors out of the box, ranging from writing to file, to displaying on screen data
tracked by each session

+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+
| :ref:`FileDumpProcessor<classwellfired_profile_profileprocessor_filedumpprocessor>`                             | Dump a file after the session is stopped                         |
+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+
| :ref:`FileStreamerProcessor<classwellfired_profile_profileprocessor_filestreamerprocessor>`                     | Streams the sessions data to disk                                |
+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+
| :ref:`NetworkDumpProcessor<classwellfired_profile_profileprocessor_networkdumpprocessor>`                       | Dumps a file over a network connection when a session is stopped |
+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+
| :ref:`NetworkStreamerProcessor<classwellfired_profile_profileprocessor_networkstreamerprocessor>`               | Streams the session data to a location over a network            |
+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+
| :ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor>`                                 | A simple built in visualiser for .Profile                        |
+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+
| :ref:`DebugLogProcessor<classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor>`               | Will Log all tracked data to the Unity Console                   |
+-----------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------+

To use one of these built in processors, simply

1) Add the required using

    .. code-block:: c#

        using WellFired.Profile.ProfileProcessor;
        using WellFired.Profile.Unity.Runtime.ProfileProcessor

2) Tell your session to use the required Processor

    .. code-block:: c#

        // Process recorded data using the built in visual display extension
        session.ProcessData(new VisualProcessor(() => Input.GetKeyDown(KeyCode.A)));

Custom Processor
----------------

.Profile provides a simple API for users who want to provide custom processors. This could be useful for customers who
wish to handle processing .Profiles data in a custom manor, for example sending tracked data to an analytics server, or
a custom endpoint.

Building custom probes is as simple as implementing the
:ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` interface.

Consider the following extension:

.. code-block:: c#

    public class CustomProcessor : IProfileProcessor
    {
        private readonly List<TimeValueTable> _timeValueTables = new List<TimeValueTable>();
        private ProbeRecorder[] _probeRecorders;

        public void RecordingStarted(ProbeRecorder[] probeRecorders)
        {
            _probeRecorders = probeRecorders;
            foreach (var probeRecorder in probeRecorders)
                _timeValueTables.Add(new TimeValueTable(probeRecorder.ProbeName()));
        }

        public void RecordingUpdated()
        {
            for (var i = 0; i < _probeRecorders.Length; i++)
            {
                if (_probeRecorders[i].Updated)
                    _timeValueTables[i].AddPoint(_probeRecorders[i].GetLastRecordedValue());
            }
        }

        public void RecordingStopped()
        {

        }
    }

Now that you have your custom processor, the last step is to tell your .Profile session to use it.

.. code-block:: c#

    session.ProcessData(new CustomProcessor());

A single session is capable of having multiple processors.