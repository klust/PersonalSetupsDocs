# Broadcast from two computers with Zoom, split sound and presentation

## Idea

-   Make it easy for the speaker to use their own laptop.
    An argument for this is that they then have their own ssh keys to show things
    live on the supercomputer.

-   And to make it easy, make sure the presenter doesn't need to take care of the sound.

-   So use two laptops:

    -   Presenter laptop:

        -   Connected directly to the screen of the room

        -   Uses Zoom with screen share

    -   Director laptop

        -   Microphone to broadcast sound

        -   Optionally: Can broadcast a camera image of the room. Viewers can then chose
            between viewing the speaker and the screen share.

        -   Optionally: Can also make the recording.


## Infrastructure for director's laptop (ideal)

-   Laptop (monitor 1), also used for the Zoom settings

-   External monitor for Zoom image, ideal for recording (monitor 2)

-   Optionally: Second external monitor that can be used to get some work done,
    like following online questions.

-   iPad is useful also to get other work done as that would not interfere.

-   So power needed: 3-4 USB-C ports + USB-A port, fits on UGreen 300W power supply

    -   USB-C for the mac, via a USB-C - to - magsafe cable
  
    -   USB-C for portable monitor used as screen 2 and connected via HDMI

    -   USB-C to charge the charging case

    -   May also want to charge the Logitech Spotlight Presenter during longer breaks just to be sure

    -   When the iPad is used to monitor the questions, USB-C or USB-A depending on the cable


## Checklists

### Packing checklists

1.  **Packing checklist: Cables**

    1.  USB-C-to-Magsafe cable provided with the macOS laptop

    2.  USB-C cable provided with the USB-C-only ASUS ZenScreen

    3.  USB-C and HDMI-to-micro-HDMI cable provided with the HDMI/USB-C ASUS ZenScreen

    4.  240V power cable to connect the USB-C power supply to a wall socket

    5.  USB-C charger cable for the microphone case

    6.  USB-C - to - lightning cable for iPad

    7.  Sometimes the extension USB-C cord may be useful for the microphone, store with the microphone.
        Otherwise it may cover multiple USB-C ports or other ports on the laptop.

2.  **Packing checklist: Other hardware**

    1.  Laptop

    2.  ASUS ZenScreen with HDMI//USB-C connector

    3.  ASUS ZenScreen USB-C only 

    4.  Logitech Pebble M350 travel mouse

    5.  USB-C power supply 300W UGreen

    6.  Consider taking an extension cord, or ask for it in advance


### Setup checklists

1.  **Hardware setup**

    1.  Laptop power: Apple UBC-C-to-Magsafe3 cable to USB-C power supply first port
        (as it is the highest power device we use)

    2.  Position of the *displays*:

        1.  Leftmost: Laptop

        2.  Middle: ASUS ZenScreen with USB-C connector only, connect to the right USB-C port
            of the laptop with the cable provided with the monitor.

        3.  Right: ASUS ZenScreen with micro-HDMI connector, connect to the HDMI splitter with
            the HDMI-to-micro-HDMI cable provided with the monitor, and to a USB-C power supply
            with the cable provided with the monitor

    3.  *Microphone*: The receiver can be connected directly to the front left USB-C port of the laptop
        as the other USB-C port is not needed so can be covered by the receiver (unless a port is needed
        for the webcam).

        Otherwise the USB-C elongation cable stored with the microphone should be used.

    4.  Connect the microphone charger case to the USB-C power supply so that it can recharge.

    5.  A regular external mouse makes life easier

    6.  The logitech presenter is very useful also to steer the presentation and show a laser pointer
        on the screen

2.  **Software setup**

    1. *What do we run where?*

       1.   Zoom controls on the laptop display. 

       2.   Zoom screen on the middle display

       3.   The right display is used as the work display (optional)

    2. *Display settings in macOS*

        1.  Reorder the displays as positioned, align the bottom.

        2.  TODO: Click on the middle display to see its settings and set the "Use as" to "main display"

        3.  You may want to play a bit with the color profile settings of particularly the projector
            screen as it looks like the mac sometimes takes them a bit on the very warm side. 

    3.  *Zoom settings*: There is a lot to check here...

        1.  Audio panel

            1.  Make sure that the microphone is properly selected. It should be either
                "Wireless Microphone RX", or if sound in macOS is properly configured to use the
                the last microphone that became available as the microphone, "Same as system
                (Wireless Microphone RX)" should also do. It may be wise to keep that window visible
                at the end.

            2.  Make sure that the checkbox to automatically adapt the volume is checked.

            3.  Letting Zoom remove background sound, seems to be perfectly fine.

            4.  You might consider to check the option towards the bottom to automatically connect
                the audio of the computer when participating in a meeting, though it is better to do that
                when starting the screen sharing.

        2.  "Screen share" panel

            1.  Standard options seem to be fine on the first screen of that panel. As we use
                desktop sharing for the meeting, some settings don't really matter.

            2.  Use the "Advanced settings" at the bottom though:

                1.  Make sure that the option to show a green border around shared content is unchecked
                    as it is very distracting

                2.  Hardware acceleration should probably remain clicked.

                3.  The modus for screen capture was left to "automatic" in our experiments.

        3.  "Recording" panel

            1.  Make sure the checkbox for showing the participants' names is unchecked (third checkbox)

            2.  Consider clicking "Optimise for video editor of third party".

            3.  Two options here, need to experiment:
   
                1.  Uncheck "Video recording while sharing screen" which might be the trick to be sure that
                    participants are not shown

                2.  Check "Video recording while sharing screen" checked and also check the box for the subchoice to
                    place the video next to the shared screen in the recording. But this only makes sense if a 
                    webcam is used.

        4.  Start Zoom once in the meeting:

            1.  Move the controls out of the way to the left screen (laptop screen)

            2.  Make sure you can start the recording.

                Shortcuts on MacOS:
                1.  Toggle start/stop the recording: Shift+command+R
                2.  Pause the recording: Shift+command+P


### During the meeting

1.  **Start-of-presentation checklist**

    1.  Check if the microphone receiver is on

    2.  Check if the sender is paired

    3.  Check if in Zoom the microphone is set to "Wireless Microphone RX" in the zoom audio panel. 
        It is not enough to check in the macOS sound panel.

    4.  Check if speaking in the microphone shows in the volume bar in the Zoom audio settings

    5.  When using a webcam, is that detected and shown?

    6.  Check if the speaker's slides are shown in the Zoom session

    7.  Check if recording is on

    8.  Check if sound in Zoom is unmuted

2.  **Extra room technician**

    1.  Preferably has a way to monitor sound in the Zoom call, e.g., via a headphone that is used
        from time to time.

    2.  Follows feedback in the Zoom chat

    3.  Follows feedback in the HedgeDoc if that is used to pass on to the speaker

    4.  Can let participants in and controls the host function

    5.  Makes a backup recording (can be done remotely also)

    6.  Ideally work on making course materials available (can be done remotely also)



