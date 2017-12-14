.. _interfacewellfired_profile_isession:

ISession
=========

**Namespace:** :ref:`WellFired<namespacewellfired>`

Description
------------

Implement this interface if you'd like to create an object that tracks probes. 

Public Methods
---------------

+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StartRecording<interfacewellfired_profile_isession_1ac70a369fea8987e748acdfacd3d499be>` **(**  **)**                                                                                                                                                                                                    |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StopRecording<interfacewellfired_profile_isession_1a1c9bf254b632487939759533a9ce0e6f>` **(**  **)**                                                                                                                                                                                                     |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<interfacewellfired_profile_isession_1a92f2983109dfe7bc4060a8e40fab5429>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**   |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<interfacewellfired_profile_isession_1ab4b775de428ad14fca84cdcf5c164802>` **(** Func< object > method, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**                                           |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<interfacewellfired_profile_isession_1a5da630902eb4c43102a0a817f1b53fd5>` **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**                                                                                                                        |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`ProcessData<interfacewellfired_profile_isession_1a7b783380bb6cc4c811a534a0691f896c>` **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**                                                                                                      |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _interfacewellfired_profile_isession_1ac70a369fea8987e748acdfacd3d499be:

- void **StartRecording** **(**  **)**

    **Description**

        Will start this profilers recording session. What is tracked and how it is process should be specify beforehand 

.. _interfacewellfired_profile_isession_1a1c9bf254b632487939759533a9ce0e6f:

- void **StopRecording** **(**  **)**

    **Description**

        Will Stop this profilers recording session. 

.. _interfacewellfired_profile_isession_1a92f2983109dfe7bc4060a8e40fab5429:

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
        
.. _interfacewellfired_profile_isession_1ab4b775de428ad14fca84cdcf5c164802:

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
        
.. _interfacewellfired_profile_isession_1a5da630902eb4c43102a0a817f1b53fd5:

- void **Track** **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**

    **Description**

        This method works similar to the Track method but record mode and interval are specified by default in the Default :ref:`Probes<namespacewellfired_profile_probes>`. You can pass one of the groups of default probes we already provide, like Defaults.All. You should prefer this method if you don't need 100% control over your probes. 

    **Parameters**

        +-------------+--------------------------------------------------------------------+
        |probes       |You can also pass one of the provided utilities like Defaults.All   |
        +-------------+--------------------------------------------------------------------+
        
.. _interfacewellfired_profile_isession_1a7b783380bb6cc4c811a534a0691f896c:

- void **ProcessData** **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**

    **Description**

        How do you want to process the data. We provide many default processors including the VisualProcessor, which will display data to the screen 

    **Parameters**

        +-------------+
        |processor    |
        +-------------+
        
