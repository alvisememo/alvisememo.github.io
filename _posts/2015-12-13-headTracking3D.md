---
layout: post
title:  "Head Tracking 3D with OpenCV"
date:   2015-10-31 00:00:00 -0800
---

Hello, in this post I want to present a small project developed with 
OpenCV for a simple head tracking with a normal webcam. By head tracking
I mean that the software tracks the user head movement in the image
taken by a camera connected to the computer (could be a webcam or
other sources). The tracking is actually a very fast and continuous
search for faces. With the acquired position of the tracked head, a
3D render is called and is used to draw on the monitor a 'fake' window
to give the tracked user the illusion of a proper projection.

The tracking and filtering of the data is done with OpenCV, the rendering
with OpenGL/FreeGLUT/GLEW.

The software workflow is as follow: 
* Init, where the Kalman filters used for smoothing the head
tracking position and other 3D model are prepared
* 3D Rendering, a loop is started and does not communicate with the
tracking side at all, except for the "SetCam" function, which specify where
the user head is, and update the viewing frustum accordingly
* Tracking, the tracking loop opens the webcam stream, and starts
tracking the first face found. When a face is found, a second classification
occours in the described area to look for two eyes, and to compute a synthetic
distance of the user from the camera.  A kalman filter is then applied both to
the x-y values, and also to the z value found before

Here a video of the result: [video](https://www.youtube.com/watch?v=X1RpwioTXjg?rel=0)

Download link to the binaries
[here](https://www.dropbox.com/s/unxwc6a96m15081/HeadTracking3D_webcam_bin.zip?dl=0),
to try this on your computer (Windows only sorry), or download the full visual studio
project (VS2012) with all included libraries
[here](https://www.dropbox.com/s/8xbsor99j6mpggk/HeadTracking3D_webcam_src.zip?dl=0).