.. _classwellfired_profile_unity_runtime_defaults:

Defaults
=========

**Namespace:** :ref:`WellFired.Profile.Unity<namespacewellfired_profile_unity>`

Description
------------

:ref:`Defaults<classwellfired_profile_unity_runtime_defaults>` provide a static access to different group of probes (All, Texture, etc...) that can be directly tracked by a :ref:`IProfile<interfacewellfired_profile_iprofile>`. 

public-static-attrib
---------------------

+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`Continuous<classwellfired_profile_unity_runtime_defaults_1a6e2ba152b3184269065046681b30e727>`                |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`ContinuousMemory<classwellfired_profile_unity_runtime_defaults_1a752974fbbcf8eaf6f6e38761d30522e7>`          |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`ContinuousObjectMemory<classwellfired_profile_unity_runtime_defaults_1a68f75c0c779261822b9b82cb9cf9e498>`    |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`Graphics<classwellfired_profile_unity_runtime_defaults_1ab9d74a3eac13230027f4f7484c19f6c8>`                  |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`GraphicsParticles<classwellfired_profile_unity_runtime_defaults_1a6a670d83c2d12884a6e2d23ffd95cf20>`         |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`GraphicsShadow<classwellfired_profile_unity_runtime_defaults_1a04737a8fd1c0819f6b3f5eb2b0ea1246>`            |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`GraphicsTexture<classwellfired_profile_unity_runtime_defaults_1a2d6924d16b3f49b81b5acaf95507006f>`           |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`Hardware<classwellfired_profile_unity_runtime_defaults_1a8f0e757e15a6b657d28422267653f7fd>`                  |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`Physics<classwellfired_profile_unity_runtime_defaults_1a57f65257da4738301431df4ca09794fa>`                   |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+
|readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` >   |:ref:`Time<classwellfired_profile_unity_runtime_defaults_1a42d2fe4a4fc81b7294ca6060666c3d4d>`                      |
+------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_unity_runtime_defaults_1a6e2ba152b3184269065046681b30e727:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **Continuous** 

    **Description**

        Static Helper allowing you to quickly track CpuLoad and Framerate 

.. _classwellfired_profile_unity_runtime_defaults_1a752974fbbcf8eaf6f6e38761d30522e7:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **ContinuousMemory** 

    **Description**

        Static Helper allowing you to quickly track generic memory usage 

.. _classwellfired_profile_unity_runtime_defaults_1a68f75c0c779261822b9b82cb9cf9e498:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **ContinuousObjectMemory** 

    **Description**

        Static Helper allowing you to quickly track object memory usage (Can be quite slow, especially in editor), better to only used this when you need it. 

.. _classwellfired_profile_unity_runtime_defaults_1ab9d74a3eac13230027f4f7484c19f6c8:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **Graphics** 

    **Description**

        Static Helper allowing you to quickly track Graphic Settings 

.. _classwellfired_profile_unity_runtime_defaults_1a6a670d83c2d12884a6e2d23ffd95cf20:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **GraphicsParticles** 

    **Description**

        Static Helper allowing you to quickly track Graphic Particle Settings 

.. _classwellfired_profile_unity_runtime_defaults_1a04737a8fd1c0819f6b3f5eb2b0ea1246:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **GraphicsShadow** 

    **Description**

        Static Helper allowing you to quickly track Graphic Shadow Settings 

.. _classwellfired_profile_unity_runtime_defaults_1a2d6924d16b3f49b81b5acaf95507006f:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **GraphicsTexture** 

    **Description**

        Static Helper allowing you to quickly track Graphic Texture Settings 

.. _classwellfired_profile_unity_runtime_defaults_1a8f0e757e15a6b657d28422267653f7fd:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **Hardware** 

    **Description**

        Static Helper allowing you to quickly track Hardware Statistics 

.. _classwellfired_profile_unity_runtime_defaults_1a57f65257da4738301431df4ca09794fa:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **Physics** 

    **Description**

        Static Helper allowing you to quickly track Physics Settings 

.. _classwellfired_profile_unity_runtime_defaults_1a42d2fe4a4fc81b7294ca6060666c3d4d:

- readonly IList< :ref:`DefaultProbe<classwellfired_profile_probes_defaultprobe>` > **Time** 

    **Description**

        Static Helper allowing you to quickly track Time Settings 

