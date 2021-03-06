.. _classwellfired_profile_unity_runtime_dotprofilesession:

DotProfileSession
==================

**Namespace:** :ref:`WellFired.Profile.Unity<namespacewellfired_profile_unity>`

Description
------------

A Utility interface that allows users to quickly obtain and manage Sessions. 

Public Static Methods
----------------------

+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
|:ref:`ISession<interfacewellfired_profile_isession>`   |:ref:`New<classwellfired_profile_unity_runtime_dotprofilesession_1ac344f4694fb28dc10071e181c10e4e85>` **(**  **)**                     |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
|void                                                   |:ref:`StartConfigProfile<classwellfired_profile_unity_runtime_dotprofilesession_1ac8def160e14194ee68deeca66e45127a>` **(**  **)**      |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
|void                                                   |:ref:`ToggleLog<classwellfired_profile_unity_runtime_dotprofilesession_1a9ff95a76cf80ae9e088e25dbc4072d64>` **(** bool enabled **)**   |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_unity_runtime_dotprofilesession_1ac344f4694fb28dc10071e181c10e4e85:

- :ref:`ISession<interfacewellfired_profile_isession>` **New** **(**  **)**

    **Description**

        Return a new :ref:`ISession<interfacewellfired_profile_isession>` allowing the caller to specify details about a what to record, when to record it and how to process that data. 

.. _classwellfired_profile_unity_runtime_dotprofilesession_1ac8def160e14194ee68deeca66e45127a:

- void **StartConfigProfile** **(**  **)**

    **Description**

        Whenever it is called, it will load *.pcfg files in StreamingAssets/DotProfileConfig/ which are files specifying what needs to be tracked and how to process it. 

.. _classwellfired_profile_unity_runtime_dotprofilesession_1a9ff95a76cf80ae9e088e25dbc4072d64:

- void **ToggleLog** **(** bool enabled **)**

    **Description**

        Toggle logs in :ref:`Unity<namespacewellfired_profile_unity>` Debug console. For debug purpose only. 

    **Parameters**

        +-------------+
        |enabled      |
        +-------------+
        
