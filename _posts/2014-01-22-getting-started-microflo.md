---
layout: documentation
title: Getting started (MicroFlo)
categories:
 - documentation
---

## Prepare your microcontroller for talking to Flowhub

To use Flowhub for programming your microcontroller, you need to flash your microcontroller
with the MicroFlo runtime and run the MicroFlo Chrome app. These steps are documented
[here](https://github.com/jonnor/microflo/blob/master/doc/arduino-getstarted.md), and need
to be completed before you continue.


## Open Flowhub Chrome app

Make sure you have Flowhub v0.2.3 or later.
Make sure your Arduino microcontroller is connected over USB.

1. Download and run the [Flowhub Chrome app](https://chrome.google.com/webstore/detail/flowhub/aacpjichompfhafnciggfpfdpfododlk)
2. Click "Login" and connect Flowhub with your TheGrid account
3. Click the refresh button next to runtimes

The MicroFlo runtime should now show up in the list of runtimes.

![runtimes list showing local MicroFlo app](../images/microflo01-runtimes.png)


## Make a project

1.  Under "Projects" click "Create"
2.  Give your project a name and label
3.  Choose "MicroFlo" as the primary type
    ![create project dialog with MicroFlo type selected](../images/microflo02-create-project.png)
4.  Tap "Create" and the UI should load, showing a blank canvas
5.  Tap "Select runtime" and chose the runtime for the serial port where your microcontroller is connected

## Make your first graph

For general help on how to use the graph creation UI, see the [Browser tutorial](../getting-started-browser).

Try to make the following Hello World graph. hit the Play/Pause to upload it to your Arduino.
Uploading will take ~1 second, and you will see the RX/TX LEDs on the board blink during this time,
as well as upload output on the left side of the UI.

![MicroFlo Hello World program: Blink](../images/microflo03-blink.png)

You should now see the LED of your Arduino blinking much faster, about 7 times a second.
If so you have a working MicroFlo for Arduino setup, and can now try to build more complicated programs!

