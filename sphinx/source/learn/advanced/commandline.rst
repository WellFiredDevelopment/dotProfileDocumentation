.. _learn_advanced_commandline:

Introduction
============

One of the more useful, but slightly more advanced functionality of .Profile is the ability to launch your application
from the command line with a selection of command line arguments allowing you to automatically start a custom recording
session. This doesn't require any code on your side, which is precisely why this functionality is so amazing, it just
works out of the box.

Usage
=====

When you install .Profile, you also install a pre configured command line profile configuration. It's located in your
project and called Framerate.pcfg. Feel free to open this and have a look at the format (it's plain Json). We'll use
this bundled configuration to show you how .Profile can leverage out of the box command line profiling.

.. warning::    .Profile ships with a link.xml file, this file tells unity not to strip out .Profile's assemblies when
                it builds a new player, it's important you have this link.xml file in your project prior to building
                your player.

1) After installing .Profile, build a player for your desired platform.
2) Run your player with the following command line arguments
::

    path/to/your/player.exe  -DotProfileConfig "Framerate"

And that's it, your application should be launched and a session will automatically be created using the Framerate.pcfg
config.

.. note::   You can create your own profile configuration files and ship them with your product, if you want to enable
            a user facing command line interface, allowing your customers the option to profile their existing game.
            Similar to how Valve ship a profiler with their hammer based products.