.. _classwellfired_profile_probes_probehashset:

ProbeHashSet
=============

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Implements:** :ref:`WellFired.Profile.Probes.IProbeCollection<interfacewellfired_profile_probes_iprobecollection>`


Description
------------



Public Properties
------------------

+-------------+----------------------------------------------------------------------------------------------------+
|int          |:ref:`ProbeCount<classwellfired_profile_probes_probehashset_1aecf45fa9a8b810f9937a856fbc63d111>`    |
+-------------+----------------------------------------------------------------------------------------------------+

Public Methods
---------------

+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|bool         |:ref:`AddProbe<classwellfired_profile_probes_probehashset_1a25ffc8be18ea9beb193505f6d8771e36>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**      |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|bool         |:ref:`RemoveProbe<classwellfired_profile_probes_probehashset_1aa4b859a6c9e838c9ba5a679a9ce6aff2>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**   |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_probes_probehashset_1aecf45fa9a8b810f9937a856fbc63d111:

- int **ProbeCount** 

.. _classwellfired_profile_probes_probehashset_1a25ffc8be18ea9beb193505f6d8771e36:

- bool **AddProbe** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**

    **Description**

        Adds a new probe to the :ref:`IProbeCollection<interfacewellfired_profile_probes_iprobecollection>`

    **Parameters**

        +-------------+-------------------+
        |probe        |The probe to add   |
        +-------------+-------------------+
        
.. _classwellfired_profile_probes_probehashset_1aa4b859a6c9e838c9ba5a679a9ce6aff2:

- bool **RemoveProbe** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**

    **Description**

        Removes a passed probe from the :ref:`IProbeCollection<interfacewellfired_profile_probes_iprobecollection>`

    **Parameters**

        +-------------+----------------------+
        |probe        |The probe to remove   |
        +-------------+----------------------+
        
