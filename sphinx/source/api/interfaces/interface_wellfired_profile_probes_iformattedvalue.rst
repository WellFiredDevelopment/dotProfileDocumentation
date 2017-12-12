.. _interfacewellfired_profile_probes_iformattedvalue:

IFormattedValue
================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

Description
------------

Optionally implement this interface if you'd like your custom probe to display data with a custom format 

Public Methods
---------------

+-------------+---------------------------------------------------------------------------------------------------------------------------------------+
|string       |:ref:`FormattedValue<interfacewellfired_profile_probes_iformattedvalue_1af61cebdfc5f6d291d313fc4c579535da>` **(** object value **)**   |
+-------------+---------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _interfacewellfired_profile_probes_iformattedvalue_1af61cebdfc5f6d291d313fc4c579535da:

- string **FormattedValue** **(** object value **)**

    **Description**

        From the probed data, return a formatted value. 

    **Parameters**

        +-------------+-----------------------------------+
        |value        |The object returned from a probe   |
        +-------------+-----------------------------------+
        
