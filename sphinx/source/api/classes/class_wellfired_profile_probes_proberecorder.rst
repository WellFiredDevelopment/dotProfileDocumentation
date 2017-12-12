.. _classwellfired_profile_probes_proberecorder:

ProbeRecorder
==============

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

Description
------------

A probe recorder contains a Probe and a Record Mode. This is used to determine what the :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>` will record and also, at what interval the recorder will refresh it's probe 

Properties
-----------

+-------------+-----------------------------------------------------------------------------------------------------------------------+
|bool         |:ref:`Updated<classwellfired_profile_probes_proberecorder_1ade3da648a3ceaaa9dfd16e1c39476583>` **{** get; set; **}**   |
+-------------+-----------------------------------------------------------------------------------------------------------------------+

Public Properties
------------------

+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------+
|readonly :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>`   |:ref:`RecordMode<classwellfired_profile_probes_proberecorder_1a0e26a81ce71530b2e0aaec2c242a317b>`    |
+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------+

Public Methods
---------------

+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|string                                                                   |:ref:`ProbeName<classwellfired_profile_probes_proberecorder_1adcef24f455c2de547c85f57a7c156a33>` **(**  **)**                                                                                                                                                                                                                                                                                                                               |
+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Type                                                                     |:ref:`ProbeType<classwellfired_profile_probes_proberecorder_1a1db61135befedc42bbf9c3cd809cc754>` **(**  **)**                                                                                                                                                                                                                                                                                                                               |
+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|                                                                         |:ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder_1a1686580285a903c06babf6d5825c2eef>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = :ref:`RecordMode.Continous<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987ac7b4a7b11db72be8e0755d14d63d0a58>`, int interval = 0 **)**   |
+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void                                                                     |:ref:`RecordSample<classwellfired_profile_probes_proberecorder_1ac613d07b1b4cdfa9b433cdc383c9c80c>` **(** long deltaTime **)**                                                                                                                                                                                                                                                                                                              |
+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|:ref:`TimeValue<structwellfired_profile_data_continousdata_timevalue>`   |:ref:`GetLastRecordedValue<classwellfired_profile_probes_proberecorder_1a42a03c18e10818e254d95b07aff927af>` **(**  **)**                                                                                                                                                                                                                                                                                                                    |
+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|:ref:`TimeValue<structwellfired_profile_data_continousdata_timevalue>`   |:ref:`GetLastFormattedRecordedValue<classwellfired_profile_probes_proberecorder_1a29f0faccec432bc26d0c27d60762fbba>` **(**  **)**                                                                                                                                                                                                                                                                                                           |
+-------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_probes_proberecorder_1ade3da648a3ceaaa9dfd16e1c39476583:

- bool **Updated** **{** get; set; **}**

    **Description**

        This flag is reset if the probe has recorded using the RecordSample method. 

.. _classwellfired_profile_probes_proberecorder_1a0e26a81ce71530b2e0aaec2c242a317b:

- readonly :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` **RecordMode** 

    **Description**

        The RecordMode that states how this Recorder will record data 

.. _classwellfired_profile_probes_proberecorder_1adcef24f455c2de547c85f57a7c156a33:

- string **ProbeName** **(**  **)**

    **Description**

        Returns the probe name for this recorder. This Probe name will either be specified on the probe or it will be specified using an :ref:`IFormattedName<interfacewellfired_profile_probes_iformattedname>` on the probe object 

.. _classwellfired_profile_probes_proberecorder_1a1db61135befedc42bbf9c3cd809cc754:

- Type **ProbeType** **(**  **)**

    **Description**

        Returns the raw type of the probe. 

.. _classwellfired_profile_probes_proberecorder_1a1686580285a903c06babf6d5825c2eef:

-  **ProbeRecorder** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = :ref:`RecordMode.Continous<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987ac7b4a7b11db72be8e0755d14d63d0a58>`, int interval = 0 **)**

    **Description**

        Constructs a new instance of :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`, by default every probe will be continuous, but if you want to optimise your probes, make sure to use Continuous only when needed. You can optionally specify the record interval, this works in conjunction with the RecordMode.Continuous, but is ignored when recordMode is OneShot 

    **Parameters**

        +-------------+---------------------------------------------+
        |probe        |The probe which we will get our data from    |
        +-------------+---------------------------------------------+
        |recordMode   |How we will record this data                 |
        +-------------+---------------------------------------------+
        |interval     |The interval that we will record this data   |
        +-------------+---------------------------------------------+
        
.. _classwellfired_profile_probes_proberecorder_1ac613d07b1b4cdfa9b433cdc383c9c80c:

- void **RecordSample** **(** long deltaTime **)**

    **Description**

        Tells the recorder to attempt to record a new sample, note this might not actually record anything, it's up to the Recorder to do the recording, calling this method is simply a way of flagging this recorder to record, if needed 

    **Parameters**

        +-------------+
        |deltaTime    |
        +-------------+
        
.. _classwellfired_profile_probes_proberecorder_1a42a03c18e10818e254d95b07aff927af:

- :ref:`TimeValue<structwellfired_profile_data_continousdata_timevalue>` **GetLastRecordedValue** **(**  **)**

    **Description**

        Returns the last recorded value as a TimeValue 

.. _classwellfired_profile_probes_proberecorder_1a29f0faccec432bc26d0c27d60762fbba:

- :ref:`TimeValue<structwellfired_profile_data_continousdata_timevalue>` **GetLastFormattedRecordedValue** **(**  **)**

    **Description**

        Rrturns the last recorded formatted value as a TimeValue 

