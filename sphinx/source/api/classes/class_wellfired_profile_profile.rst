.. _classwellfired_profile_profile:

Profile
========

**Namespace:** :ref:`WellFired<namespacewellfired>`

**Implements:** :ref:`WellFired.Profile.IProfile<interfacewellfired_profile_iprofile>`


Description
------------

Our basic profiler object 

Public Methods
---------------

+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`Profile<classwellfired_profile_profile_1a98296301ef712094ec3e4e3a0e587e43>` **(**  **)**                                                                                                                                                                                                           |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`Profile<classwellfired_profile_profile_1a704b6c4a23c3689dfa64f22d88a805e4>` **(** :ref:`ITimer<interfacewellfired_profile_probes_itimer>` timer, :ref:`IRuntimeTaskLooper<interfacewellfired_profile_utils_iruntimetasklooper>` runtimeTaskLooper **)**                                            |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<classwellfired_profile_profile_1a33c15d24aad1166760af53ecf44f6eae>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**   |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<classwellfired_profile_profile_1ae205bdbfad58db67aa4aea09c7a73b79>` **(** Func< object > method, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**                                           |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<classwellfired_profile_profile_1a843479e08d4862532dfd5c93bf01be16>` **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**                                                                                                                        |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`ProcessData<classwellfired_profile_profile_1aac3e0d9f94d83b38aae7824e17a708ed>` **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**                                                                                                      |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StartRecording<classwellfired_profile_profile_1a7ac756f2b006b3d806168815372731d0>` **(**  **)**                                                                                                                                                                                                    |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StopRecording<classwellfired_profile_profile_1a162767d8ac15f511c533ccabc5e69f6c>` **(**  **)**                                                                                                                                                                                                     |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Method Breakdown
-----------------

.. _classwellfired_profile_profile_1a98296301ef712094ec3e4e3a0e587e43:

-  **Profile** **(**  **)**

    **Description**

        Creates a new instance of :ref:`Profile<classwellfired_profile_profile>`, with default settings, you'll likely only need to call this 

.. _classwellfired_profile_profile_1a704b6c4a23c3689dfa64f22d88a805e4:

-  **Profile** **(** :ref:`ITimer<interfacewellfired_profile_probes_itimer>` timer, :ref:`IRuntimeTaskLooper<interfacewellfired_profile_utils_iruntimetasklooper>` runtimeTaskLooper **)**

    **Description**

        Creates a new instance of :ref:`Profile<classwellfired_profile_profile>` allowing you to provide a custom timer and task looper 

    **Parameters**

        +--------------------+
        |timer               |
        +--------------------+
        |runtimeTaskLooper   |
        +--------------------+
        
.. _classwellfired_profile_profile_1a33c15d24aad1166760af53ecf44f6eae:

- void **Track** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**

    **Description**

        Tracks a given probe, with the passed data 

    **Parameters**

        +-------------+----------------------------------------------------------------------+
        |probe        |The probe that we should track                                        |
        +-------------+----------------------------------------------------------------------+
        |recordMode   |The record mode to use when we're getting tracked data                |
        +-------------+----------------------------------------------------------------------+
        |interval     |The interval that we would like to use when retrieving tracked data   |
        +-------------+----------------------------------------------------------------------+
        
.. _classwellfired_profile_profile_1ae205bdbfad58db67aa4aea09c7a73b79:

- void **Track** **(** Func< object > method, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**

    **Description**

        Allows you to track custom data on this profiler, simply pass the method that will extract the custom data as the first parameter 

    **Parameters**

        +-------------+----------------------------------------------------------------------+
        |method       |A delegate that will be used to extract custom data                   |
        +-------------+----------------------------------------------------------------------+
        |recordMode   |The record mode to use when we're getting tracked data                |
        +-------------+----------------------------------------------------------------------+
        |interval     |The interval that we would like to use when retrieving tracked data   |
        +-------------+----------------------------------------------------------------------+
        
.. _classwellfired_profile_profile_1a843479e08d4862532dfd5c93bf01be16:

- void **Track** **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**

    **Description**

        Tracks a collection of probes. 

    **Parameters**

        +-------------+
        |probes       |
        +-------------+
        
.. _classwellfired_profile_profile_1aac3e0d9f94d83b38aae7824e17a708ed:

- void **ProcessData** **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**

    **Description**

        How do you want to process the data. We provide many default processors including the VisualProcessor, which will display data to the screen 

    **Parameters**

        +-------------+
        |processor    |
        +-------------+
        
.. _classwellfired_profile_profile_1a7ac756f2b006b3d806168815372731d0:

- void **StartRecording** **(**  **)**

    **Description**

        Start Recording :ref:`Data<namespacewellfired_profile_data>`

.. _classwellfired_profile_profile_1a162767d8ac15f511c533ccabc5e69f6c:

- void **StopRecording** **(**  **)**

    **Description**

        Stop recording data 

