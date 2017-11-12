.. _class_WellFired.Profile.Profile:

WellFired.Profile.Profile
=========================

**Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`

**Namespace:** :ref:`WellFired.Profile<namespace_WellFired.Profile>`

Description
-----------

Our basic profiler object

Member Functions
----------------

+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`Profile<class_WellFired.Profile.Profile__Profile>` **(** **)**                                                                                                                                                                 |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`Profile<class_WellFired.Profile.Profile__Profile_ITimer_IRuntimeTaskLooper>` **(** :ref:`ITimer<interface_ITimer>` timer , :ref:`IRuntimeTaskLooper<interface_IRuntimeTaskLooper>` runtimeTaskLooper **)**                     |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`Track<class_WellFired.Profile.Profile__Track_IProbe_RecordMode_int>` **(** :ref:`IProbe<interface_IProbe>` probe, :ref:`RecordMode<enum_RecordMode>` recordMode = RecordMode.Continuous, int interval = 0 **)**                |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`Track<class_WellFired.Profile.Profile__Track_Funcobj_RecordMode_int>` **(** Func<object> method, :ref:`RecordMode<enum_RecordMode>` recordMode = RecordMode.Continuous, int interval = 0 **)**                                 |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`Track<class_WellFired.Profile.Profile__Track_IEnumerable_defaultprobe>` **(** IEnumerable<:ref:`DefaultProbe<class_DefaultProbe>`> probes **)**                                                                                |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`ProcessData<class_WellFired.Profile.Profile__ProcessData>` **(** :ref:`IProfileProcessor<interface_IProfileProcessor>` processor **)**                                                                                         |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`StartRecording<class_WellFired.Profile.Profile__StartRecording>` **(** **)**                                                                                                                                                   |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                               | :ref:`StopRecording<class_WellFired.Profile.Profile__StopRecording>` **(** **)**                                                                                                                                                     |
+------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Member Function Description
---------------------------

.. _class_WellFired.Profile.Profile__Profile:

- void **Profile** **(** **)**

    **Description**
    
        Creates a new instance of :ref:`Profile<class_WellFired.Profile.Profile>`, with default settings, you'll likely only need to call this

.. _class_WellFired.Profile.Profile__Profile_ITimer_IRuntimeTaskLooper:

- void **Profile** **(** :ref:`ITimer<interface_ITimer>` timer , :ref:`IRuntimeTaskLooper<interface_IRuntimeTaskLooper>` runtimeTaskLooper **)**

    **Description**
    
        Creates a new instance of :ref:`Profile<class_WellFired.Profile.Profile>`, allowing you to provide a custom timer and task looper

.. _class_WellFired.Profile.Profile__Track_IProbe_RecordMode_int:

- void **Track** **(** :ref:`IProbe<interface_IProbe>` probe, :ref:`RecordMode<enum_RecordMode>` recordMode = RecordMode.Continuous, int interval = 0 **)** 

    **Description**

        Tracks a given :ref:`IProbe<interface_IProbe>`, with the passed data

    **Parameters**

        +--------------+----------------------+-----------------------------------------------+
        | probe        | The probe that we should track.                                      |
        +--------------+----------------------+-----------------------------------------------+
        | recordMode   | The record mode to use when we're getting tracked data               |
        +--------------+----------------------+-----------------------------------------------+
        | interval     | The interval that we would like to use when retrieving tracked data  |
        +--------------+----------------------+-----------------------------------------------+

    **Exceptions**

        +----------------------------------------------------------+---------------------------------------------------------------------+
        | :ref:`ProbeAlreadyAdded<class_ProbeAlreadyAdded>`        | This probe has likely already been added                            |
        +----------------------------------------------------------+---------------------------------------------------------------------+

    **Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`

.. _class_WellFired.Profile.Profile__Track_Funcobj_RecordMode_int:

- void **Track** **(** Func<object> method, :ref:`RecordMode<enum_RecordMode>` recordMode = RecordMode.Continuous, int interval = 0 **)**        

    **Description**
    
        Allows you to track custom data on this profiler, simply pass the method that will extract the custom data as the first parameter

        Call this to track the data returned by one of your method.

    **Parameters**

        +--------------+----------------------+-----------------------------------------------+
        | method       | A delegate that will be used to extract custom data                  |
        +--------------+----------------------+-----------------------------------------------+
        | recordMode   | The record mode to use when we're getting tracked data               |
        +--------------+----------------------+-----------------------------------------------+
        | interval     | The interval that we would like to use when retrieving tracked data  |
        +--------------+----------------------+-----------------------------------------------+

    **Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`

.. _class_WellFired.Profile.Profile__Track_IEnumerable_defaultprobe:

- void **Track** **(** IEnumerable<:ref:`DefaultProbe<class_DefaultProbe>`> probes **)**

    **Description**
    
        Tracks a collection of probes.

        This method works similar to the Track method but record mode and interval are specified by default in the Default Probes. You can pass one of the groups of default probes we already provide, like Defaults.All. You should prefer this method if you don't need 100% control over your probes.

    **Parameters**

        +--------------+----------------------+-----------------------------------------------+
        | probes       | The probes that we should track.                                     |
        +--------------+----------------------+-----------------------------------------------+

    **Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`

.. _class_WellFired.Profile.Profile__ProcessData:

- void **ProcessData** **(** :ref:`IProfileProcessor<interface_IProfileProcessor>` processor **)**

    **Description**
    
        How do you want to process the data. We provide many default processors including the VisualProcessor, which will display data to the screen

    **Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`

.. _class_WellFired.Profile.Profile__StartRecording:

- void **StartRecording** **(** **)**

    **Description**
    
        Starts Recording Data

    **Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`

.. _class_WellFired.Profile.Profile__StopRecording:

- void **StopRecording** **(** **)**

    **Description**
    
        Stops Recording Data

    **Implements:** :ref:`IProfile<interface_WellFired.Profile.IProfile>`