Session
=======

Introduction
------------

A session is a simple construct that refers to the start and end of a recording session. This recording session takes
Probes as inputs and Processors as outputs (More on that in the coming pages).

Managing a session
------------------

A Session object is required to manage a session, a session can be constructed by hand, but we provide a simple
interface for users to easily initialise a session. You can do this with the following steps.

1) Add the required using

    .. code-block:: c#

        using WWellFired.Profile.Unity.Runtime;

2) Tell your session to track the data you require.

    .. code-block:: c#

        var session = DotProfileSession.New();

Now you've got a session, you should start it when you want to start recording data.

    .. code-block:: c#

        session.StartRecording();

You can also tell your session to stop recording when you don't require it to record anymore.

    .. code-block:: c#

        session.StopRecording();

.. tip:: In these examples, we show you how to use and manage a single session, but it's important to mention you're
         not limited to just one, you can create as many as you want / need.

Sessions will automatically stop recording when your application terminates, but we provide the functionality for you
to stop them, in case you want to manage your sessions in a custom manor.

Next up
-------

Sessions are a small topic, with not many functions, but they're the cornerstone of your recording process. We're going
to teach you how to make them more useful in the coming pages.