.. _classwellfired_profile_probes_customprobe:

CustomProbe
============

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Implements:** :ref:`WellFired.Profile.Probes.IProbe<interfacewellfired_profile_probes_iprobe>`, :ref:`WellFired.Profile.Probes.IFormattedName<interfacewellfired_profile_probes_iformattedname>`


Description
------------

A custom Probe can be used if you want to add custom data to your profiling session. 

Properties
-----------

+-------------+------------------------------------------------------------------------------------------------------------------+
|string       |:ref:`Name<classwellfired_profile_probes_customprobe_1acc1f52c31445da02c5a8a7409c4fd544>` **{** get; set; **}**   |
+-------------+------------------------------------------------------------------------------------------------------------------+

Public Methods
---------------

+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
|             |:ref:`CustomProbe<classwellfired_profile_probes_customprobe_1ac1fec19c41e75999fa9e8a51e3564ef4>` **(** Func< object > method, string name **)**   |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
|object       |:ref:`Probe<classwellfired_profile_probes_customprobe_1ac8ea37bc6dca2bf702b9dd212acd6c01>` **(**  **)**                                           |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_probes_customprobe_1acc1f52c31445da02c5a8a7409c4fd544:

- string **Name** **{** get; set; **}**

.. _classwellfired_profile_probes_customprobe_1ac1fec19c41e75999fa9e8a51e3564ef4:

-  **CustomProbe** **(** Func< object > method, string name **)**

    **Description**

        Constructs a new instance of :ref:`CustomProbe<classwellfired_profile_probes_customprobe>`

    **Parameters**

        +-------------+-----------------------------------------------+
        |method       |The method that will return your custom data   |
        +-------------+-----------------------------------------------+
        |name         |Name this probe something sensible             |
        +-------------+-----------------------------------------------+
        
.. _classwellfired_profile_probes_customprobe_1ac8ea37bc6dca2bf702b9dd212acd6c01:

- object **Probe** **(**  **)**

    **Description**

        Returns the probed data. 

