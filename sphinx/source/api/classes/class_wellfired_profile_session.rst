.. _classwellfired_profile_session:

Session
========

**Namespace:** :ref:`WellFired<namespacewellfired>`

**Implements:** :ref:`WellFired.Profile.ISession<interfacewellfired_profile_isession>`


Description
------------

Our basic profiler object 

Public Methods
---------------

+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`Session<classwellfired_profile_session_1a944150937742007af79657dd3c093d64>` **(**  **)**                                                                                                                                                                                                           |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`Session<classwellfired_profile_session_1a758c24d6042844b2124bd2ceb9406147>` **(** :ref:`ITimer<interfacewellfired_profile_probes_itimer>` timer, :ref:`IRuntimeTaskLooper<interfacewellfired_profile_utils_iruntimetasklooper>` runtimeTaskLooper **)**                                            |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<classwellfired_profile_session_1a67c47fadeb5864336232d9ca72fd4a65>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**   |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<classwellfired_profile_session_1a994ea11b30c6ecb0254a993c79e5f1b5>` **(** Func< object > method, :ref:`RecordMode<namespacewellfired_profile_probes_1a3a8dc0a82edb0eba6bb423fbc8910987>` recordMode = RecordMode.Continous, int interval = 0 **)**                                           |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`Track<classwellfired_profile_session_1ac5c14e82289086d4f8630e105c2f404b>` **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**                                                                                                                        |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`ProcessData<classwellfired_profile_session_1a43ab5aaffeb1be83feac31fe5e23f7ef>` **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**                                                                                                      |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StartRecording<classwellfired_profile_session_1a06067b46037c62c25bc780e754218a6a>` **(**  **)**                                                                                                                                                                                                    |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`StopRecording<classwellfired_profile_session_1a26a75f3e6f016b37b55a9cb44c1c5a64>` **(**  **)**                                                                                                                                                                                                     |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_session_1a944150937742007af79657dd3c093d64:

-  **Session** **(**  **)**

    **Description**

        Creates a new instance of :ref:`Profile<namespacewellfired_profile>`, with default settings, you'll likely only need to call this 

.. _classwellfired_profile_session_1a758c24d6042844b2124bd2ceb9406147:

-  **Session** **(** :ref:`ITimer<interfacewellfired_profile_probes_itimer>` timer, :ref:`IRuntimeTaskLooper<interfacewellfired_profile_utils_iruntimetasklooper>` runtimeTaskLooper **)**

    **Description**

        Creates a new instance of :ref:`Profile<namespacewellfired_profile>` allowing you to provide a custom timer and task looper 

    **Parameters**

        +--------------------+
        |timer               |
        +--------------------+
        |runtimeTaskLooper   |
        +--------------------+
        
.. _classwellfired_profile_session_1a67c47fadeb5864336232d9ca72fd4a65:

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
        
.. _classwellfired_profile_session_1a994ea11b30c6ecb0254a993c79e5f1b5:

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
        
.. _classwellfired_profile_session_1ac5c14e82289086d4f8630e105c2f404b:

- void **Track** **(** IEnumerable< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > probes **)**

    **Description**

        Tracks a collection of probes. 

    **Parameters**

        +-------------+
        |probes       |
        +-------------+
        
.. _classwellfired_profile_session_1a43ab5aaffeb1be83feac31fe5e23f7ef:

- void **ProcessData** **(** :ref:`IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>` processor **)**

    **Description**

        How do you want to process the data. We provide many default processors including the VisualProcessor, which will display data to the screen 

    **Parameters**

        +-------------+
        |processor    |
        +-------------+
        
.. _classwellfired_profile_session_1a06067b46037c62c25bc780e754218a6a:

- void **StartRecording** **(**  **)**

    **Description**

        Start Recording :ref:`Data<namespacewellfired_profile_data>`

.. _classwellfired_profile_session_1a26a75f3e6f016b37b55a9cb44c1c5a64:

- void **StopRecording** **(**  **)**

    **Description**

        Stop recording data 

