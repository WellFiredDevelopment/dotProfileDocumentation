.. _classwellfired_profile_profileprocessor_fileprocessor:

FileProcessor
==============

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Implements:** :ref:`WellFired.Profile.ProfileProcessor.IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>`


Description
------------

This is an abstract implementation of a FileStreamProcessor 

protected-attrib
-----------------

+----------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
|readonly Stream                                                       |:ref:`Stream<classwellfired_profile_profileprocessor_fileprocessor_1af37c09b2728758116e49586d9b7a0656>`               |
+----------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
|:ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[]   |:ref:`ProbeRecorders<classwellfired_profile_profileprocessor_fileprocessor_1af1ee9cf31ec88088e77638a1647e03a4>`       |
+----------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
|readonly bool                                                         |:ref:`StreamSetManually<classwellfired_profile_profileprocessor_fileprocessor_1a3d0e7850681b8389ea81619292ee41bb>`    |
+----------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+

protected-func
---------------

+-------------+-------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`FileProcessor<classwellfired_profile_profileprocessor_fileprocessor_1ae5d7925377a55f3a4115c85af9b9cc99>` **(** Stream stream **)**   |
+-------------+-------------------------------------------------------------------------------------------------------------------------------------------+

Public Methods
---------------

+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void            |:ref:`RecordingStarted<classwellfired_profile_profileprocessor_fileprocessor_1a2390b53195a38db17b9fd07c03c3089c>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**   |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void            |:ref:`RecordingUpdated<classwellfired_profile_profileprocessor_fileprocessor_1a2fe9d973df26bbd5268297da0403d92c>` **(**  **)**                                                                                     |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|abstract void   |:ref:`RecordingStopped<classwellfired_profile_profileprocessor_fileprocessor_1abae8de0c8698d24161ec7d2faeaa4e1d>` **(**  **)**                                                                                     |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_profileprocessor_fileprocessor_1af37c09b2728758116e49586d9b7a0656:

- readonly Stream **Stream** 

.. _classwellfired_profile_profileprocessor_fileprocessor_1af1ee9cf31ec88088e77638a1647e03a4:

- :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] **ProbeRecorders** 

.. _classwellfired_profile_profileprocessor_fileprocessor_1a3d0e7850681b8389ea81619292ee41bb:

- readonly bool **StreamSetManually** 

.. _classwellfired_profile_profileprocessor_fileprocessor_1ae5d7925377a55f3a4115c85af9b9cc99:

-  **FileProcessor** **(** Stream stream **)**

.. _classwellfired_profile_profileprocessor_fileprocessor_1a2390b53195a38db17b9fd07c03c3089c:

- void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_fileprocessor_1a2fe9d973df26bbd5268297da0403d92c:

- void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_profileprocessor_fileprocessor_1abae8de0c8698d24161ec7d2faeaa4e1d:

- abstract void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

