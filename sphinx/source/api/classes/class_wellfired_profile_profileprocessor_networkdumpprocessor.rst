.. _classwellfired_profile_profileprocessor_networkdumpprocessor:

NetworkDumpProcessor
=====================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Implements:** :ref:`WellFired.Profile.ProfileProcessor.IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>`


Description
------------

A custom Processor that will dump your data over a network. 

Public Methods
---------------

+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`NetworkDumpProcessor<classwellfired_profile_profileprocessor_networkdumpprocessor_1aed353238473b34a74b9848d557beb0f5>` **(** string address, Protocol protocol = Protocol.TCP **)**                                  |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStarted<classwellfired_profile_profileprocessor_networkdumpprocessor_1a4914425d6ebf6cf98de882b4c9525543>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>` [] probeRecorders **)**   |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingUpdated<classwellfired_profile_profileprocessor_networkdumpprocessor_1a414f88b93778d02edb35da3520655796>` **(**  **)**                                                                                      |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStopped<classwellfired_profile_profileprocessor_networkdumpprocessor_1a4387ff64c24004b5fe3e135bdc6e5ca4>` **(**  **)**                                                                                      |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Method Breakdown
-----------------

.. _classwellfired_profile_profileprocessor_networkdumpprocessor_1aed353238473b34a74b9848d557beb0f5:

-  **NetworkDumpProcessor** **(** string address, Protocol protocol = Protocol.TCP **)**

    **Description**

        Creates a new instance of :ref:`NetworkDumpProcessor<classwellfired_profile_profileprocessor_networkdumpprocessor>`

    **Parameters**

        +-------------+--------------------------------------------+
        |address      |The Ip you'd like to dump to.               |
        +-------------+--------------------------------------------+
        |protocol     |The Protocol you want to use when dumping   |
        +-------------+--------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_networkdumpprocessor_1a4914425d6ebf6cf98de882b4c9525543:

- void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>` [] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_networkdumpprocessor_1a414f88b93778d02edb35da3520655796:

- void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_profileprocessor_networkdumpprocessor_1a4387ff64c24004b5fe3e135bdc6e5ca4:

- void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

