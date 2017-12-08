.. _interfacewellfired_profile_probes_iprobecollection:

IProbeCollection
=================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

Description
------------

A probe collection is a collection of probes. 

Properties
-----------

+-------------+------------------------------------------------------------------------------------------------------------------------+
|int          |:ref:`ProbeCount<interfacewellfired_profile_probes_iprobecollection_1a769449ae94766ffdad919ad7df858afc>` **(**  **)**   |
+-------------+------------------------------------------------------------------------------------------------------------------------+

Public Methods
---------------

+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|bool         |:ref:`AddProbe<interfacewellfired_profile_probes_iprobecollection_1a9cfbe8cadd2d669a4f7ef0cff555909c>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**      |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|bool         |:ref:`RemoveProbe<interfacewellfired_profile_probes_iprobecollection_1ad59fbfd9d77a8298a2cff01dc913ca9c>` **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**   |
+-------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Method Breakdown
-----------------

.. _interfacewellfired_profile_probes_iprobecollection_1a769449ae94766ffdad919ad7df858afc:

- int **ProbeCount** **(**  **)**

    **Description**

        How many probes are in this collection. 

.. _interfacewellfired_profile_probes_iprobecollection_1a9cfbe8cadd2d669a4f7ef0cff555909c:

- bool **AddProbe** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**

    **Description**

        Adds a new probe to the :ref:`IProbeCollection<interfacewellfired_profile_probes_iprobecollection>`

    **Parameters**

        +-------------+-------------------+
        |probe        |The probe to add   |
        +-------------+-------------------+
        
.. _interfacewellfired_profile_probes_iprobecollection_1ad59fbfd9d77a8298a2cff01dc913ca9c:

- bool **RemoveProbe** **(** :ref:`IProbe<interfacewellfired_profile_probes_iprobe>` probe **)**

    **Description**

        Removes a passed probe from the :ref:`IProbeCollection<interfacewellfired_profile_probes_iprobecollection>`

    **Parameters**

        +-------------+----------------------+
        |probe        |The probe to remove   |
        +-------------+----------------------+
        
