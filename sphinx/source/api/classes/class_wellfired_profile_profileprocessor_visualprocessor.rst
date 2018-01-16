.. _classwellfired_profile_profileprocessor_visualprocessor:

VisualProcessor
================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Implements:** :ref:`WellFired.Profile.ProfileProcessor.IProfileProcessor<interfacewellfired_profile_profileprocessor_iprofileprocessor>`


Description
------------

A custom processor that has a visual representation 

Properties
-----------

+---------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
|:ref:`GraphConfig<classwellfired_profile_profileprocessor_visual_graph_graphconfig>`   |:ref:`GraphConfig<classwellfired_profile_profileprocessor_visualprocessor_1ac2bcb42858c86bd08d27b1cd6f4092f1>` **{** get; set; **}**   |
+---------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+

Public Methods
---------------

+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor_1ab458270b1bf70ea3e92a4bde57b3bcbc>` **(** Func< bool > toggleUIFunc, IEnumerable< Type > additionalProbeTypesToProbeToGraph **)**                                                                                                                                            |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor_1a5b951c549fa167cfddd877cd7fac7689>` **(** IEnumerable< Type > additionalProbeTypesToProbeToGraph **)**                                                                                                                                                                       |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor_1a56968736492e22dbcd8df2f3a653b607>` **(**  **)**                                                                                                                                                                                                                             |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor_1ade0d3304004daf75b1c84b2080453e6a>` **(** Func< bool > toggleUIFunc **)**                                                                                                                                                                                                    |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor_1aded3d174f5c313ebadcfe1e658c77849>` **(** :ref:`IUILoader<interfacewellfired_profile_profileprocessor_visual_group_iuiloader>` uiLoader, Func< bool > toggleUIFunc, :ref:`IRuntimeTaskLooper<interfacewellfired_profile_utils_iruntimetasklooper>` runtimeTaskLooper **)**   |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStarted<classwellfired_profile_profileprocessor_visualprocessor_1aaaa859c0ea0864b0372db3d246922b84>` **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**                                                                                                                                          |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingUpdated<classwellfired_profile_profileprocessor_visualprocessor_1a8775435f673315e5c8246d24dc65e23e>` **(**  **)**                                                                                                                                                                                                                            |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|void         |:ref:`RecordingStopped<classwellfired_profile_profileprocessor_visualprocessor_1a4f604836b79977681d617d218f011069>` **(**  **)**                                                                                                                                                                                                                            |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_profileprocessor_visualprocessor_1ac2bcb42858c86bd08d27b1cd6f4092f1:

- :ref:`GraphConfig<classwellfired_profile_profileprocessor_visual_graph_graphconfig>` **GraphConfig** **{** get; set; **}**

    **Description**

        This gives you access to the different parameters to configure your graph. Note that once your :ref:`Profile<namespacewellfired_profile>` session started, any modification to the graph config won't have any impact. 

.. _classwellfired_profile_profileprocessor_visualprocessor_1ab458270b1bf70ea3e92a4bde57b3bcbc:

-  **VisualProcessor** **(** Func< bool > toggleUIFunc, IEnumerable< Type > additionalProbeTypesToProbeToGraph **)**

    **Description**

        Constructs a new instance of :ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor>`. 

    **Parameters**

        +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        |toggleUIFunc                         |An optional delegate that controls the display of the :ref:`Visual<namespacewellfired_profile_profileprocessor_visual>` Processor. This delegate should return true whenever you want to toggle the display state of the UI.   |
        +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        |additionalProbeTypesToProbeToGraph   |An option IEnumerable of additional probe types to add to the graph                                                                                                                                                            |
        +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_visualprocessor_1a5b951c549fa167cfddd877cd7fac7689:

-  **VisualProcessor** **(** IEnumerable< Type > additionalProbeTypesToProbeToGraph **)**

    **Description**

        Constructs a new instance of :ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor>`. 

    **Parameters**

        +-------------------------------------+----------------------------------------------------------------------+
        |additionalProbeTypesToProbeToGraph   |An option IEnumerable of additional probe types to add to the graph   |
        +-------------------------------------+----------------------------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_visualprocessor_1a56968736492e22dbcd8df2f3a653b607:

-  **VisualProcessor** **(**  **)**

    **Description**

        Constructs a new instance of :ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor>`. 

.. _classwellfired_profile_profileprocessor_visualprocessor_1ade0d3304004daf75b1c84b2080453e6a:

-  **VisualProcessor** **(** Func< bool > toggleUIFunc **)**

    **Description**

        Constructs a new instance of :ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor>`. 

    **Parameters**

        +---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        |toggleUIFunc   |An optional delegate that controls the display of the :ref:`Visual<namespacewellfired_profile_profileprocessor_visual>` Processor. This delegate should return true whenever you want to toggle the display state of the UI.   |
        +---------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_visualprocessor_1aded3d174f5c313ebadcfe1e658c77849:

-  **VisualProcessor** **(** :ref:`IUILoader<interfacewellfired_profile_profileprocessor_visual_group_iuiloader>` uiLoader, Func< bool > toggleUIFunc, :ref:`IRuntimeTaskLooper<interfacewellfired_profile_utils_iruntimetasklooper>` runtimeTaskLooper **)**

    **Description**

        Constructs a new instance of :ref:`VisualProcessor<classwellfired_profile_profileprocessor_visualprocessor>`

    **Parameters**

        +--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
        |uiLoader            |The object which deals with loading the UI                                                                                                              |
        +--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
        |toggleUIFunc        |A delegate that will deal with toggling the visual display. This delegate should return true whenever you want to toggle the display state of the UI.   |
        +--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
        |runtimeTaskLooper   |                                                                                                                                                        |
        +--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_visualprocessor_1aaaa859c0ea0864b0372db3d246922b84:

- void **RecordingStarted** **(** :ref:`ProbeRecorder<classwellfired_profile_probes_proberecorder>`[] probeRecorders **)**

    **Description**

        The Record has been started 

    **Parameters**

        +-----------------+--------------------------------------------------+
        |probeRecorders   |This recording session will record these probes   |
        +-----------------+--------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_visualprocessor_1a8775435f673315e5c8246d24dc65e23e:

- void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_profileprocessor_visualprocessor_1a4f604836b79977681d617d218f011069:

- void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

