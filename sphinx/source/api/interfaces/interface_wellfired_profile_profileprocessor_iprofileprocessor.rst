.. _interfacewellfired_profile_profileprocessor_iprofileprocessor:

IProfileProcessor
==================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

Description
------------

Implement this interface if you want to provide custom profile processors. For example, you could use this functionality if you wanted to create a custom analytics processor, sending all recorded data to an analytics provider, for instance. 

Public Methods
---------------

+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStarted<interfacewellfired_profile_profileprocessor_iprofileprocessor_1a63014de04422ce240af7262d991eb247>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**   |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingUpdated<interfacewellfired_profile_profileprocessor_iprofileprocessor_1a1beee3dc6428a9d9a19fba7adbfbf2fa>` **(**  **)**                                                                                     |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStopped<interfacewellfired_profile_profileprocessor_iprofileprocessor_1a02e42a69827f623c5a917a2a917fc846>` **(**  **)**                                                                                     |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _interfacewellfired_profile_profileprocessor_iprofileprocessor_1a63014de04422ce240af7262d991eb247:

- void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _interfacewellfired_profile_profileprocessor_iprofileprocessor_1a1beee3dc6428a9d9a19fba7adbfbf2fa:

- void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _interfacewellfired_profile_profileprocessor_iprofileprocessor_1a02e42a69827f623c5a917a2a917fc846:

- void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

