Probes
======

Introduction
------------

A probe is a simple construct that allows you to extract data from your game and give it to .Profile. A single .Profile
session can having multiple probes into your application. This allows you as a developer a way to keep your game
code an your .Profile code separated from one another, imposing a semi strict seperation of concerns.

.Profile ships with a whole bunch of Default :ref:`Probes<classwellfired_profile_unity_runtime_defaults>` that allow
you to instantly probe most functionality that Unity provides. These Probes are available out of the box and can be
used.

All Probes used by .Profile fall into one of two categories

* Continuous probes
    These probes continually probe your application at a specified interval, these probes can be useful for data that
    changes over time, such as framerate or memory usage

* One shot probes
    One shot probes will probe your app once and once only, these probes can be useful for data that won't change at
    runtime, such as hardware stats.

Provided Probes
---------------

.Profiles Default :ref:`Probes<classwellfired_profile_unity_runtime_defaults>` are split fairly evenly between
continuous and one shot probes. Out of the box, .Profile provides probes for the following data.

+-----------------------------------+----------------------+----------------------------------------------+
| Name                              | Probe Type           | Tracks                                       |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.Continuous               | Continuous           | CPU load and framerate                       |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.ContinuousMemory         | Continuous           | Memory usage across many systems             |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.ContinuousObjectMemory   | Continuous           | Memory in use by various GameObjects         |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.Graphics                 | One Shot             | The current graphics settings                |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.GraphicsParticles        | One Shot             | The current graphics settings for particles  |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.GraphicsShadow           | One Shot             | The current graphics settings for shadows    |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.GraphicsTexture          | One Shot             | The current graphics settings for textures   |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.Hardware                 | One Shot             | The current hardware settings                |
+-----------------------------------+----------------------+----------------------------------------------+
| Defaults.Time                     | One Shot             | The current time settings                    |
+-----------------------------------+----------------------+----------------------------------------------+

To use one of these Default :ref:`Probes<classwellfired_profile_unity_runtime_defaults>`, simply

1) Add the required using

    .. code-block:: c#

        using WellFired.Profile.ProfileProcessor;

2) Tell your session to track the data you require.

    .. code-block:: c#

        // Track Continuous memory usage
        session.Track(Defaults.ContinuousMemory);


Custom Probes
-------------

.Profile provides a simple API for users who want to provide custom probes, allowing users to track any custom data in
their application.

Building custom probes is as simple as implementing the :ref:`IProbe<interfacewellfired_profile_probes_iprobe>`
interface.

consider the following simple custom probe that doesn't do anything other than return the float 60.

.. code-block:: c#

    public class CustomProbe : IProbe
    {
        /// <summary>
        /// Return a value
        /// </summary>
        /// <returns>Always returns 60</returns>
        public object Probe()
        {
            return 60.0f;
        }
    }

The :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` interface requires you implement the Probe method. From this
method you are required to return your custom tracked data, this can be anything you want it to be, it doesn't even have
to be performance related (maybe a custom in-game currency spent over time).

Further to this simple example, you can also implement the
:ref:`IFormattedName<interfacewellfired_profile_probes_iformattedname>` interface, this gives you a method for naming
your probe, but is entirely optional.

consider the following extensions:

.. code-block:: c#

    public class CustomProbe : IProbe, IFormattedName
    {
        /// <summary>
        /// Return a value
        /// </summary>
        /// <returns>Always returns 60</returns>
        public object Probe()
        {
            return 60.0f;
        }

        /// <summary>
        /// The IFormattedName is optional
        /// </summary>
        public string Name { get { return "Custom Probe"; } }
    }

Now that you have your custom probe, the last step is to tell your .Profile session to track it.

.. code-block:: c#

    session.Track(new CustomProbe(), RecordMode.Continous, 100);

When Tracking a custom probe, you are required to tell your session if it should be probed continuously or only once and
at what interval. This corresponds to the second and third parameter respectively.

Next up
-------

Now we've covered tracking data using built in probes and writing custom probes to track custom application logic and
data, we'll cover reporting that data.