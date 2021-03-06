# leap-motion-monitor

The Leap Motion Monitor is a [Processing 3](https://processing.org/) application that shows real-time charts of time series of a number of [Leap Motion](https://www.leapmotion.com/) measures. The following image shows the application in action. The left column shows the time series for the left hand, the right column for those for the right hand. Nine measures are shown for each hand: palm position (3 axis), palm rotation (3 axis), grab strength, pinch strength and extended finger count.

[![Screenshot](img/screen_1.png)](img/screen_1.png)

The initial purpose of this application was to monitor the aforementioned Leap Motion measures and inspect strategies for stabilising these time series such that they become more usable for interactive generative purposes. A control panel allows the user to disable the use the stabilised palm position data. The user can also disable additional stabilisation and smoothing (by bounding the first derivative) of the time series. The individual values are marked with dots and color coded according to type. Values that were smoothed or interpolated are marked as red dots.

# Running the application

Obviously you need a Leap Motion to enjoy this application. You will also need to install Processing 3 to execute this application.

This application uses two libraries: the [_LeapMotion_](ttps://github.com/heuermh/leap-motion-processing) library by Michael Heuer and the [_Control5P_](http://www.sojamo.de/libraries/controlP5/reference/) library by Andreas Schlegel. The _LeapMotion_ library provides a simple integration of the [_Leap Motion Java API_](https://developer.leapmotion.com/documentation/java/api/Leap_Classes.html) in Processing.

Both libraries are available in the library manager in Processing 3. To install these library, select _Sketch_ in the Processing application/window menu, then _Import Library..._ and _Add Library..._. Now select the library and click on the Install button. Do this for both libraries.

# License

Copyright (c) 2015, Wouter Van den Broeck

Leap Motion Monitor is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

Leap Motion Monitor is distributed in the hope that it will be
useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Leap Motion Monitor.  If not, see [http://www.gnu.org/licenses/](http://www.gnu.org/licenses/).