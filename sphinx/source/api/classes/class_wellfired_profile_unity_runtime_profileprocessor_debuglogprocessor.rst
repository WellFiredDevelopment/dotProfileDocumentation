.. _classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor:

DebugLogProcessor
==================

**Namespace:** :ref:`WellFired.Profile.Unity.Runtime<namespacewellfired_profile_unity_runtime>`

**Implements:** :ref:`WellFired.Profile.ProfileProcessor.IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>`


Description
------------

A custom Processor that prints all profiler information to the debug console. 

Public Methods
---------------

+-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStarted<classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor_1a262080e92579524b84d7cd4db7a46d01>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**   |
+-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingUpdated<classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor_1a82227058be11b141652f0234733c407a>` **(**  **)**                                                                                     |
+-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStopped<classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor_1acd57409de9a3717538518cd9c18fd1bc>` **(**  **)**                                                                                     |
+-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor_1a262080e92579524b84d7cd4db7a46d01:

- void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor_1a82227058be11b141652f0234733c407a:

- void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_unity_runtime_profileprocessor_debuglogprocessor_1acd57409de9a3717538518cd9c18fd1bc:

- void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

