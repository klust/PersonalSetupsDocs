# Broadcast via OBS from a second PC (either Zoom or YouTube/Twitch/...)

## Idea

-   Make it easy for the presenter to use their own laptop.
    An argument for this is that they then have their own ssh keys to show things
    live on the supercomputer.

-   And a director takes care of all work of the broadcast. This may even including
    switching to a room camera view or mixing a slide with the camera view in the corner.


## Common setup

### Packing checklist

#### Extra cables

1.  USB-C-to-magsafe cable to feed the Apple laptop
2.  USB-C-to-Lightning cable to feed the iPad
3.  Longer HDMI cable to connect the capture device to the laptop of the presenter.
4.  USB-C-to-USB-C cable to connect to the DJI mic receiver, should be included with the DJI mic.
5.  USB-C-to-USB-C power cable for the DJI Mic case.
6.  If extra monitors are taken along, make sure you also take the cables for them (USB-C, or USB-C + HDMI-to-micro-HDMI).
7.  Optional: If the conference microphone is used to capture sound from the room: Long (5m) USB-C-to-USB-C cable.
8.  Optional: When webcam is used, 5m USB-C-female-to-USB-C-male extension cable for the webcam. Only works with the better webcam though as it is a USB-C cable.
9.  Power extension cord is often useful if there is no size and weight problem.


#### Other hardware

1.  Laptop
2.  Useful but optional: iPad to steer OBS
3.  Logitech Pebble mouse
4.  USB hub to connect USB-A devices (Elgato, webcam depending on which webcam is used)
5.  Power supply UGreen 200W + power cable
6.  DJI microphone
7.  Elgato HD60x, which comes with a short HDMI-to-HDMI cable and a short USB-C-to-USB-A cable to
    connect the device to a USB-A port (the Elgato has a USB-C connector)
8.  Portable screen 1080p with HDMI is very useful as feedback from the HDMI splitter and to force
    it in a resolution that is processed well by the Elgato.
9.  Extra screen for laptop as the screen real estate is small. Can be the Minisforum monitor.
10. Optional but very useful: HDMI splitter: Connect laptop of presenter to input, and extra HDMI monitor, projector and HDMI capture to outputs.
11. Optional: Conference microphone
12. Optional: Webcam + tripod
13. Optional: JBL Bluetooth speaker


## Common hardware setup for option 1 and option 2

-   One USB-C port to connect to an extra monitor so that the HDMI port remains free to project from the laptop also.

-   Connecting the video capture device of a second USB-C port
  
    -   Without HDMI splitter, which implies without extra HDMI monitor

        -   HDX60 to laptop with the USB-C cable included in the bag of the HDX60.

        -   Presenter's laptop to HDX60 "HDMI IN" with the HDMI cable in the bag of the HDX60 or the longer one if available.

        -   Projector cable in HDX60 "HDMI OUT"

    -   With HDMI splitter

        -   Power bric of HDMI splitter to power the HDMI splitter

        -   Presenter's laptop to the "Input" of the HDMI splitter with either the short cable included with the splitter or a longer HDMI cable.

        -   1080p HDMI monitor to "Output 1" of the HDMI splitter

            -   Power from the UGreen power bric.

        -   Projector to "Output 2" of the HDMI splitter with the HDMI cable of the projector

        -   HDX60 "HDMI IN" to "Output 3" of the splitter with the HDMI cable in the bag of the HDX60

        -   HDX60 to laptop with the USB-C cable included in the bag of the HDX60.

-   USB-C port 3: Microphones and webcam

    -   When connecting more than one device: Use the Satechi USB-C hub with 3 USB-C ports and an ethernet port

    -   DJI microphone:

        -   Receiver on mini-tripod stored with the UGreen power supply

        -   USB-C-to-USB-C cable in the bag of the microphone to connect to the receiver

        -   Short USB-C-to-USB-A cable in the bag of the microphone can be used to charge the case of the microphones

    -   Conference microphone Tonor TM20: Connect with the longer USB-C-to-USB-C cable as its own cable is USB-C-to-USB-A.

    -   Webcam:

        -   Connect directly

        -   Or connect via the USB-C-female-to-USB-C-male extension cable


## Option 1: Broadcast to YouTube or a similar OBS-supported service software setup



## Option 2: Broadcast to Zoom software setup

### Software needed

-   [OBS](https://obsproject.com/)
  
-   VB-Cable [virtual audio cable software from vb-audio.com](https://vb-audio.com/Cable/index.htm)

-   [Audio Hijack](https://rogueamoeba.com/audiohijack/) is useful also and needed to redirect the 
    Zoom output to the JBL speaker while still being able to present from the laptop and send the 
    system audio to OBS.


### Software setup

1.  What do we run where?

    -   OBS and Audio Hijack on the laptop.

    -   When presenting from the same laptop, use HDMI to the HDX60 and make sure sound also goes there.


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

        4.  Connect the speaker to VB-Cable B if you want Zoom output to the recording and possibly to the 
            JBL speaker (the latter with Audio Hijack).  


### Web links with information

-   [AnyRec page "Connect OBS to Zoom: Webcam, Audio Output, and Live Stream"](https://www.anyrec.io/obs-to-zoom/)



