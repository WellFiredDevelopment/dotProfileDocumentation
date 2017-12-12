.. _interfacewellfired_profile_iprofile:

IProfile
=========

**Namespace:** :ref:`WellFired<namespacewellfired>`

Description
------------

Implement this interface if you'd like to create an object that tracks probes. 

Public Methods
---------------

+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StartRecording<interfacewellfired_profile_iprofile_1aee366237f48ae0bfc0afe49ac587583c>` **(**  **)**                                                                                                                                                                                                    |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StopRecording<interfacewellfired_profile_iprofile_1aab8b82b829d662d7c72d988527e9c8e0>` **(**  **)**                                                                                                                                                                                                     |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<interfacewellfired_profile_iprofile_1aae6556095115643f579b6cc750f17f4d>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**   |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<interfacewellfired_profile_iprofile_1a3fcd45eda3f5cc9e756ae62f251d466a>` **(** Func< object > method, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**                                           |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<interfacewellfired_profile_iprofile_1a68df2fe9da924f5ccf6e95d0c7747b7b>` **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**                                                                                                                        |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`ProcessData<interfacewellfired_profile_iprofile_1a009f3be1178abab7390c3571221f0f75>` **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**                                                                                                      |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _interfacewellfired_profile_iprofile_1aee366237f48ae0bfc0afe49ac587583c:

- void **StartRecording** **(**  **)**

    **Description**

        Will start this profilers recording session. What is tracked and how it is process should be specify beforehand 

.. _interfacewellfired_profile_iprofile_1aab8b82b829d662d7c72d988527e9c8e0:

- void **StopRecording** **(**  **)**

    **Description**

        Will Stop this profilers recording session. 

.. _interfacewellfired_profile_iprofile_1aae6556095115643f579b6cc750f17f4d:

- void **Track** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**

    **Description**

        Call this to specify the probes you want to use to track data. You can add custom probes here, or any of the many pre-created probes. You can record probes continuously or only once when the session is just started (one-shot mode). If you just want an easy to use interface, you can prefer the to use Track(IEnumerable probes) 

    **Parameters**

        +-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
        |probe        |Here you can pass any probes you want to track.                                                                                                        |
        +-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
        |recordMode   |Continous or One-Shot recording                                                                                                                        |
        +-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
        |interval     |Time interval between each data sampling. Note that the time used is based on the system clock, therefore it is independent from the game time scale   |
        +-------------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
        
.. _interfacewellfired_profile_iprofile_1a3fcd45eda3f5cc9e756ae62f251d466a:

- void **Track** **(** Func< object > method, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**

    **Description**

        Call this to track the data returned by one of your method. 

    **Parameters**

        +-------------+
        |method       |
        +-------------+
        |recordMode   |
        +-------------+
        |interval     |
        +-------------+
        
.. _interfacewellfired_profile_iprofile_1a68df2fe9da924f5ccf6e95d0c7747b7b:

- void **Track** **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**

    **Description**

        This method works similar to the Track method but record mode and interval are specified by default in the Default :ref:`Probes<namespacewellfired_profile_probes>`. You can pass one of the groups of default probes we already provide, like Defaults.All. You should prefer this method if you don't need 100% control over your probes. 

    **Parameters**

        +-------------+--------------------------------------------------------------------+
        |probes       |You can also pass one of the provided utilities like Defaults.All   |
        +-------------+--------------------------------------------------------------------+
        
.. _interfacewellfired_profile_iprofile_1a009f3be1178abab7390c3571221f0f75:

- void **ProcessData** **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**

    **Description**

        How do you want to process the data. We provide many default processors including the VisualProcessor, which will display data to the screen 

    **Parameters**

        +-------------+
        |processor    |
        +-------------+
        
