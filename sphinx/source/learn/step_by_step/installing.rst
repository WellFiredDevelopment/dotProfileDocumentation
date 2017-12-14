.. _learn_step_by_step_installation:

Installing
==========

Package Contents
----------------
Each .unitypackage downloaded from the store or from the `WellFired <https://www.wellfired.com>`_ website will have the
same contents.

* \/WellFired
    Here you're going to find all things related to the .Profile project.
* /link.xml
    This file contains a list of assemblies that might be needed if your Unity Project enables stripping. This will
    ensure Unity doesn't remove needed assemblies.
* /Bootstrap.cs
    This is a simple script that you can attach to a game object and have instant profile support. Feel free to
    investigate this script, this script should be well commented and give you a solid base.

Dependencies
------------

.Profile has two dependencies, both come included with the installation, however they might conflict with your already
existing project, especially if it's a large project, the following assemblies are included with .Profile.

* `NewtonSoft.Json <https://www.newtonsoft.com/json>`_
    This isn't the typical NewtonSoft.Json package, it's a custom build package that doesn't use JIT compilation,
    making it the preferred choice if you plan to target none desktop platforms. It's prepared and developed by
    WellFired, but it runs against all of Newtonsoft.Jsons unit tests. Prefer this over your installation if you don't
    want `NewtonSoft.Json <https://www.newtonsoft.com/json>`_ to use to use JIT compilation.

* WellFired.Promise
    A lightweight promise library.

.. tip:: If either of these assemblies conflict with your project, removing them won't harm .Profile, .Profile will
         simply default to using the versions contained in your project.

Installing
----------

1. Import the .unitypackage into your unity project.
2. Add the scene WellFired/WellFired.Profile/VisualAssets/Scenes/DotProfileUI to your build settings if you'd like to
   recieve our automatic performance visualisation.

To be continued.....
--------------------

This section walked you through installing .Profile, in the next section you'll get to use .Profile with our pre made
script.