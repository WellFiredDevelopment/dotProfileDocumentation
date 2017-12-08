.. _classwellfired_profile_unity_runtime_dotprofile:

DotProfile
===========

**Namespace:** :ref:`WellFired.Profile.Unity<namespacewellfired_profile_unity>`

Description
------------

Provides a set of Utility methods that allow the user to quickly instantiate and use Profilers, without having to think about platform specific implementations. 

Public Static Methods
----------------------

+-------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------+
|:ref:`IProfile<interfacewellfired_profile_iprofile>`   |:ref:`New<classwellfired_profile_unity_runtime_dotprofile_1a3a6e3b7095890eb4274adb0098d0b150>` **(**  **)**                     |
+-------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------+
|void                                                   |:ref:`StartConfigProfile<classwellfired_profile_unity_runtime_dotprofile_1a96f78d2eff3d1543dd7901830446c086>` **(**  **)**      |
+-------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------+
|void                                                   |:ref:`ToggleLog<classwellfired_profile_unity_runtime_dotprofile_1a071a6aa2be8ce836ffa4242815d4426a>` **(** bool enabled **)**   |
+-------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------+

Method Breakdown
-----------------

.. _classwellfired_profile_unity_runtime_dotprofile_1a3a6e3b7095890eb4274adb0098d0b150:

- :ref:`IProfile<interfacewellfired_profile_iprofile>` **New** **(**  **)**

    **Description**

        Return a profile allowing to specify details about a record session (data to track, how to process it) and start then stop it. 

.. _classwellfired_profile_unity_runtime_dotprofile_1a96f78d2eff3d1543dd7901830446c086:

- void **StartConfigProfile** **(**  **)**

    **Description**

        Whenever it is called, it will load *.pcfg files in StreamingAssets/DotProfileConfig/ which are files specifying what needs to be tracked and how to process it. 

.. _classwellfired_profile_unity_runtime_dotprofile_1a071a6aa2be8ce836ffa4242815d4426a:

- void **ToggleLog** **(** bool enabled **)**

    **Description**

        Toggle logs in :ref:`Unity<namespacewellfired_profile_unity>` Debug console. For debug purpose only. 

    **Parameters**

        +-------------+
        |enabled      |
        +-------------+
        
