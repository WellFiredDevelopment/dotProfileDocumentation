.. _classwellfired_profile_profileprocessor_networkstreamerprocessor:

NetworkStreamerProcessor
=========================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Implements:** :ref:`WellFired.Profile.ProfileProcessor.IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>`


Description
------------



Public Methods
---------------

+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`NetworkStreamerProcessor<classwellfired_profile_profileprocessor_networkstreamerprocessor_1a30d2dba966dc0c0988b6dd45e731da53>` **(** string address, Protocol protocol = Protocol.TCP **)**                             |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStarted<classwellfired_profile_profileprocessor_networkstreamerprocessor_1a57eda83e12048e8dc4815baaa29890d5>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**   |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingUpdated<classwellfired_profile_profileprocessor_networkstreamerprocessor_1a4ebda255b7cdf8276ec705e25987d574>` **(**  **)**                                                                                     |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStopped<classwellfired_profile_profileprocessor_networkstreamerprocessor_1a769008aec3d1c82bf0fc1d178889f5e6>` **(**  **)**                                                                                     |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_profileprocessor_networkstreamerprocessor_1a30d2dba966dc0c0988b6dd45e731da53:

-  **NetworkStreamerProcessor** **(** string address, Protocol protocol = Protocol.TCP **)**

.. _classwellfired_profile_profileprocessor_networkstreamerprocessor_1a57eda83e12048e8dc4815baaa29890d5:

- void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_networkstreamerprocessor_1a4ebda255b7cdf8276ec705e25987d574:

- void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_profileprocessor_networkstreamerprocessor_1a769008aec3d1c82bf0fc1d178889f5e6:

- void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

