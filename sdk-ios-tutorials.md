# iOS tutorials

# Welcome to the GStreamer SDK iOS tutorials

These tutorials describe iOS-specific topics. General GStreamer concepts
will not be explained in these tutorials, so the [Basic
tutorials](http://docs.gstreamer.com/display/GstSDK/Basic+tutorials) should
be reviewed first. The reader should also be familiar with basic iOS
programming techniques.

The iOS tutorials have the same structure as the [Android
tutorials](Android%2Btutorials.html): Each one builds on top of the
previous one and adds progressively more functionality, until a working
media player application is obtained in [iOS tutorial 5: A Complete
media
player](http://docs.gstreamer.com/display/GstSDK/iOS+tutorial+5%3A+A+Complete+media+player).

Make sure to have read the instructions in [Installing for iOS
development](Installing%2Bfor%2BiOS%2Bdevelopment.html) before jumping
into the iOS tutorials.

All iOS tutorials are split into the following classes:

  - The `GStreamerBackend` class performs all GStreamer-related tasks
    and offers a simplified interface to the application, which does not
    need to deal with all the GStreamer details. When it needs to
    perform any UI action, it does so through a delegate, which is
    expected to adhere to the `GStreamerBackendDelegate` protocol.
  - The `ViewController` class manages the UI, instantiates the
    `GStreamerBackend` and also performs some UI-related tasks on its
    behalf.
  - The `GStreamerBackendDelegate` protocol defines which methods a
    class can implement in order to serve as a UI delegate for the
    `GStreamerBackend`.