.. _classwellfired_profile_unity_runtime_configs_jsonconfigloader:

JsonConfigLoader
=================

**Namespace:** :ref:`WellFired.Profile.Unity.Runtime<namespacewellfired_profile_unity_runtime>`

**Implements:** :ref:`WellFired.Profile.Config.Utils.IJSONConfigLoader<interfacewellfired_profile_config_utils_ijsonconfigloader>`


Description
------------

Loads a config file from the DotProfileConfig directory 

Public Methods
---------------

+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
|string       |:ref:`LoadJsonConfig<classwellfired_profile_unity_runtime_configs_jsonconfigloader_1a21f9677d8765260b909aadb050f5ac5f>` **(** string fileName **)**   |
+-------------+------------------------------------------------------------------------------------------------------------------------------------------------------+

Method Breakdown
-----------------

.. _classwellfired_profile_unity_runtime_configs_jsonconfigloader_1a21f9677d8765260b909aadb050f5ac5f:

- string **LoadJsonConfig** **(** string fileName **)**

    **Description**

        Load the actual config, returning the loaded data before deserialization 

    **Parameters**

        +-------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        |fileName     |The file you'd like to load, the file does not need to have the .pcfg extension. the file also does not need to be a full path, the fileName provided should be relative to the DotProfileConfig directory. I.E. If you want SomeDirectory/AnotherDirectory/DotProfileCOnfig/ConfigFile.pcfg, the fileName used should be ConfigFile.   |
        +-------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
        
