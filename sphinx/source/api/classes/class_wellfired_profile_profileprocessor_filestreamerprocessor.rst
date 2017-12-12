.. _classwellfired_profile_profileprocessor_filestreamerprocessor:

FileStreamerProcessor
======================

**Namespace:** :ref:`WellFired.Profile<namespacewellfired_profile>`

**Inherits:** :ref:`WellFired.Profile.ProfileProcessor.FileProcessor<classwellfired_profile_profileprocessor_fileprocessor>`


Description
------------

A custom :ref:`Profile<classwellfired_profile_profile>` Processor that will stream your profiled data to disk. Use this variation if you're worried about your application not exiting cleanly, otherwise, use the :ref:`FileProcessor<classwellfired_profile_profileprocessor_fileprocessor>`

Public Methods
---------------

+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------+
|                |:ref:`FileStreamerProcessor<classwellfired_profile_profileprocessor_filestreamerprocessor_1af65d93f76df4e779d1a298d6ac22032b>` **(** string filepath **)**   |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------+
|                |:ref:`FileStreamerProcessor<classwellfired_profile_profileprocessor_filestreamerprocessor_1aae97ba41097ea1667aaca09361c2baff>` **(** Stream stream **)**     |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------+
|override void   |:ref:`RecordingUpdated<classwellfired_profile_profileprocessor_filestreamerprocessor_1ae7f0efe2c009d50c225573101270ad82>` **(**  **)**                       |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------+
|override void   |:ref:`RecordingStopped<classwellfired_profile_profileprocessor_filestreamerprocessor_1a3d4bc6b69f409983d04c052406dfdc17>` **(**  **)**                       |
+----------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------+

Breakdown
----------

.. _classwellfired_profile_profileprocessor_filestreamerprocessor_1af65d93f76df4e779d1a298d6ac22032b:

-  **FileStreamerProcessor** **(** string filepath **)**

    **Description**

        Constructs a new instance of a :ref:`FileStreamerProcessor<classwellfired_profile_profileprocessor_filestreamerprocessor>`. 

    **Parameters**

        +-------------+-------------------------------------------------------+
        |filepath     |The file you'd like to dump your recording data into   |
        +-------------+-------------------------------------------------------+
        
.. _classwellfired_profile_profileprocessor_filestreamerprocessor_1aae97ba41097ea1667aaca09361c2baff:

-  **FileStreamerProcessor** **(** Stream stream **)**

    **Description**

        Constructs a new instance of :ref:`FileStreamerProcessor<classwellfired_profile_profileprocessor_filestreamerprocessor>`, use this variation if you'd like to manage your own stream. 

    **Parameters**

        +-------------+
        |stream       |
        +-------------+
        
.. _classwellfired_profile_profileprocessor_filestreamerprocessor_1ae7f0efe2c009d50c225573101270ad82:

- override void **RecordingUpdated** **(**  **)**

    **Description**

        The recording data has been updated. 

.. _classwellfired_profile_profileprocessor_filestreamerprocessor_1a3d4bc6b69f409983d04c052406dfdc17:

- override void **RecordingStopped** **(**  **)**

    **Description**

        The recording has stopped. 

