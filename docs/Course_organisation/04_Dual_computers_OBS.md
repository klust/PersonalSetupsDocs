# Broadcast via OBS from a second PC (either Zoom or YouTube/Twitch/...)

## Idea

-   Make it easy for the speaker to use their own laptop.
    An argument for this is that they then have their own ssh keys to show things
    live on the supercomputer.

-   And a director takes care of all work of the broadcast. This may even including
    switching to a room camera view or mixing a slide with the camera view in the corner.


## Common setup

### Packing checklist

#### Extra cables

1.  USB-C-to-magsafe cable to feed the laptop
2.  USB-C-to-Lightning cable to feed the iPad
3.  Longer HDMI cable to connect the capture device to the laptop of the presenter.
4.  Extension cable for the DJI mic, should be included with the DJI mic
5.  USB-C-to-USB-C power cable for the DJI Mic case
6.  If extra monitors are taken along, make sure you also take the cables for them (USB-C, or USB-C + HDMI-to-micro-HDMI)
7.  Optional: When webcam is used, extension cable for the webcam. Only works with the better webcam though as it is a USB-C cable.
8.  Power extension cord is often useful if there is no size and weight problem.


#### Other hardware

1.  Laptop
2.  iPad to steer OBS
3.  Logitech Pebble mouse
4.  USB hub to connect USB-A devices (Elgato, webcam depending on which webcam is used)
5.  Power supply 300W + power cable
6.  DJI microphone
7.  Optional: One or two extra monitors can help.
8.  Elgato HD60x, which comes with a short HDMI-to-HDMI cable and a short USB-C-to-USB-A cable to
    connect the device to a USB-A port (the Elgato has a USB-C connector)
9.  Optional: Webcam + tripod


## Option 1: Broadcast to YouTube or a similar OBS-supported service



## Option 2: Broadcast to Zoom



### Setup checklist

#### Hardware setup


#### Software setup

1.  What do we run where?

2.  Special setup of OBS and Zoom

    1.  OBS needs to have the virtual camera plugin installed and activated. macOS security may protest
        at first, but the plugin is built-in in recent macOS versions of OBS.

        1.  macOS settings app: Go to "General" → "Login Items & Extensions" → Camera Extensions"
        2.  Make sure that this is on. It may make sense to toggle it off and on if the virtual camera
            does not work when you try to activate it in OBS.

            See [Virtual Camera Troubleshooting](https://obsproject.com/kb/virtual-camera-troubleshooting)

    2.  OBS needs a virtual cable for sound output to Zoom.

        1.  Download and install the [virtual audio cable software from vb-audio.com](https://vb-audio.com/Cable/index.htm)
   
        2.  In OBS, you need to set the virtual audio cable as the monitoring device

            1.  Go to "Settings" in the right bottom of the screen

            2.  Select "Audio" and scroll down to the "Advanced" section

            3.  Set "Monitoring Device" to "VB-Cable".

            4.  On the main screen of OBS, right-click Audio Mixer and select Advanced Audio Properties. 

            5.  Set all audio sources to "Monitor and Output" to ensure that they are sent to the monitor device and regular output.

    3.  Zoom needs to connect to the virtual camera and VB-Cable device

        1.  In "Video", select "OBS Virtual Camera" as the camera

        2.  In "Audio", select "VB-Cable" as the microphone

        3.  In "Background/Effects", ensure that there is no virtual background as that will screw up everything.


### Web links with information

-   [AnyRec page "Connect OBS to Zoom: Webcam, Audio Output, and Live Stream"](https://www.anyrec.io/obs-to-zoom/)



