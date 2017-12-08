.. _classwellfired_profile_profileprocessor_filedumpprocessor:

FileDumpProcessor
==================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Inherits:** :ref:`WellFired.Profile.ProfileProcessor.FileProcessor<classwellfired_profile_profileprocessor_fileprocessor>`


Description
------------

A custom Processor that will dump all recorded data to disk once the recording has stopped. If you want to get all data regardless of application success or failure, you might consider using the FileStreamProcessor 

Public Methods
---------------

+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|                |:ref:`FileDumpProcessor<classwellfired_profile_profileprocessor_filedumpprocessor_1a79b8e2e9d73009f9cd0c56e9913af2ea>` **(** string filepath **)**                                                                      |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|                |:ref:`FileDumpProcessor<classwellfired_profile_profileprocessor_filedumpprocessor_1a27becf4c60c6a2acf3bf06cef06a612b>` **(** Stream stream **)**                                                                        |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|override void   |:ref:`RecordingStarted<classwellfired_profile_profileprocessor_filedumpprocessor_1af7dc0311f466796cd237871cf7972e61>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>` [] probeRecorders **)**   |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|override void   |:ref:`RecordingUpdated<classwellfired_profile_profileprocessor_filedumpprocessor_1ae3ca675ce3f7834fcf4fc3a07fd11676>` **(**  **)**                                                                                      |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|override void   |:ref:`RecordingStopped<classwellfired_profile_profileprocessor_filedumpprocessor_1aad7b1ffcecc150611ddc277400a50711>` **(**  **)**                                                                                      |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Method Breakdown
-----------------

.. _classwellfired_profile_profileprocessor_filedumpprocessor_1a79b8e2e9d73009f9cd0c56e9913af2ea:

-  **FileDumpProcessor** **(** string filepath **)**

    **Description**

        Constructs a new :ref:`FileDumpProcessor<classwellfired_profile_profileprocessor_filedumpprocessor>`. 

    **Parameters**

        +-------------+-------------------------------------------------------+
        |filepath     |The file you'd like to dump your recording data into   |
        +-------------+-------------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_filedumpprocessor_1a27becf4c60c6a2acf3bf06cef06a612b:

-  **FileDumpProcessor** **(** Stream stream **)**

    **Description**

        Constructs a new :ref:`FileDumpProcessor<classwellfired_profile_profileprocessor_filedumpprocessor>`, use this variant if you want to manage the Stream yourself. 

    **Parameters**

        +-------------+
        |stream       |
        +-------------+
        
.. _classwellfired_profile_profileprocessor_filedumpprocessor_1af7dc0311f466796cd237871cf7972e61:

- override void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>` [] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_filedumpprocessor_1ae3ca675ce3f7834fcf4fc3a07fd11676:

- override void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_profileprocessor_filedumpprocessor_1aad7b1ffcecc150611ddc277400a50711:

- override void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

