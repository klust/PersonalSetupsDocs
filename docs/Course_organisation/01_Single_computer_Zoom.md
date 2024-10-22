# Direct broadcast on Zoom from a single computer

## Main problems to expect

-   Get the sound right while being able to swap laptops easily.

    For this reason we have always  connected the microphone to a second laptop
    and broadcast sound from a second laptop.

    This option is really only suited if every presenter uses the same laptop as
    switching is too complicated unless all laptops are set up before to use the
    microphone.

-   Get sound from videos on Zoom

    **Method 1** for this is done when starting the screen sharing.
    In the right column of the screen sharing window (where you select which screen to share),
    you'll see a check box "Share sound" that should be clicked, and there should also be
    a second check box "Optimize for video clip" which may also be useful.

    **Method 2** is via the "Audio" settings panel of Zoom. Towards the bottom there is an option
    to automatically connect the audio of the computer when participating to a meeting.

-   Zoom puts a green border around the screen it is sharing

    **Solution:** In the "Screen sharing" settings screen, select "Advanced options" and then
    unclick the option to display the green border.   

-   It is important to get the recordings settings right.

    -   Keep "Record video while sharing screen" clicked?

    -   Unclick the option to share the names of the participants in the recording.

    -   Maybe select "Optimize for video-editor of third party"

-   PowerPoint cannot set the screen for speaker presentation, only the screen for the 
    display of the presentation. The presenter view is always shown on the laptop screen,
    even when the presentation is started from another screen or the laptop screen is not
    the leftmost monitor.

    **Solution**: In the macOS screen settings, click the display that you want as the main
    display and set it to "Main display" in the box under the display orderning.


## Infrastructure (ideal)

-   Laptop (first monitor)

-   HDMI switch, connect laptop to switch, then switch to projector and to second monitor 
    that serves as a control screen

-   Third monitor is useful also. Takes 1 USB-C port

-   Microphone, takes a USB-C port

-   Power needed:

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

    4.  A short HDMI cable (connect laptop to splitter)

    5.  Splitter power supply with cable

    6.  Cable with the USB-C power supply to connect to a wall socket

    7.  USB-C charger cable for the microphone case

    8.  Sometimes the extension USB-C cord may be useful for the microphone, store with the microphone.
        Otherwise it may cover multiple USB-C ports or other ports on the laptop.

2.  **Packing checklist: Other hardware**

    1.  Laptop

    2.  ASUS ZenScreen with HDMI//USB-C connector and cables

    3.  ASUS ZenScreen USB-C only

    4.  Logitech Pebble M350 travel mouse

    5.  Logitech Presenter

    6.  A USB-C-to-USB-C cable that is flat enough to charge the Logitech Sportlight Presenter, or a charger with 
        USB-A connection.

    7.  NEDIS 1-to-4 HDMI splitter with its power supply

    8.  USB-C power supply

    9.  Consider taking an extension cord, or ask for it in advance


### Setup checklists

1.  **Hardware setup**

    1.  Laptop power: Apple UBC-C-to-Magsafe3 cable to USB-C power supply first port
        (as it is the highest power device we use)

    2.  Switch setup (NEDIS 1-to-4 splitter)

        1.  Use a short HDMI cable to connect the switch to the HDMI port of the laptop

        2.  HDMI 1 will be used for the ASUS display. This should be enough to force 1080p

        3.  Connect the projector to the second HDMI output

    3.  Position of the *displays*:

        1.  Leftmost: Laptop

        2.  Middle: ASUS ZenScreen with USB-C connector only, connect to the right USB-C port
            of the laptop with the cable provided with the monitor.

        3.  Right: ASUS ZenScreen with micro-HDMI connector, connect to the HDMI splitter with
            the HDMI-to-micro-HDMI cable provided with the monitor, and to a USB-C power supply
            with the cable provided with the monitor

    4.  *Microphone*: The receiver can be connected directly to the front left USB-C port of the laptop
        as the other USB-C port is not needed so can be covered by the receiver.

        Otherwise the USB-C elongation cable stored with the microphone should be used.

    5.  Connect the microphone charger case to the USB-C power supply so that it can recharge.

    6.  A regular external mouse makes life easier

    7.  The logitech presenter is very useful also to steer the presentation and show a laser pointer
        on the screen

2.  **Software setup**

    1. *What do we run where?*

       1.   Zoom controls on the laptop display. 

       2.   PowerPoint on the middle display

       3.   The right display is used as the display on which the presentation is shown

    2. *Display settings in macOS*

        1.  Reorder the displays as positioned, align the bottom.

        2.  Click on the middle display to see its settings and set the "Use as" to "main display"

        3.  You may want to play a bit with the color profile settings of particularly the projector
            screen as it looks like the mac sometimes takes them a bit on the very warm side. 

    3.  *Sound settings in macOS*

        1.  It appears that the sound output device should be "ZoomAudioDevice" to be able to 
            transmit sound to the Zoom recording and call. If not, the sound will actually be 
            picked up by the microphone and you cannot mute the sound of the microphone.

    4.  *Zoom settings*: There is a lot to check here...

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

            3.  I left "Video recording while sharing screen" checked and the box for the subchoice to
                place the video next to the shared screen in the recording, unchecked.

        4.  Start Zoom once in the meeting:

            1.  Start the screen share:

                1.  Select "Desktop 3" as the screen to share

                2.  To the right, ensure that "Sharing sound" is clicked if you want to play videos with sound

                3.  Consider also selecting "Optimise for videoclip".

            2.  Move the controls out of the way to the left screen (laptop screen)

            3.  If you go with the mouse over the green zone "you're sharing your screen", more controls will
                appear. Under "More" you can start the recording.

                Shortcuts on MacOS:
                1.  Toggle start/stop the recording: Shift+command+R
                2.  Pause the recording: Shift+command+P
   
                Note that there is some visual feedback on the green bar, as it shows a flashing red dot 
                surrounded by a circle when recording and two red bars surrounded by a circle when paused.

    5.  *PowerPoint settings*

        1.  "Slide Show" - "Aangepaste voorstelling" or "Set up slide show" and set the monitor for 
            the slide show to "Monitor 3" (at the bottom of that box). The type should be set to
            "Presented by a speaker" which is the first choice, at the top of the box.

        2.  It looks like all work should be done in Zoom first before starting the presentation
            as otherwise the presenter mouse does not function.

            Tip: Long-press the "next slide" button on the presenter mouse as it has been set to
            start the presentation from the current slide, and this seems to ensure also that the forward
            and backward buttons will work properly afterwards. 


### During the meeting

1.  **Start-of-presentation checklist**

    1.  Check if the receiver is on

    2.  Check if the sender is paired

    3.  Check if in Zoom the microphone is set to "Wireless Microphone RX" in the zoom audio panel. 
        It is not enough to check in the macOS sound panel.

    4.  Check if speaking in the microphone shows in the volume bar in the Zoom audio settings

    5.  Check the sound output settings on the Mac, especially if you want to play video and hence
        are sharing the sound with Zoom. Are they set to the Zoom virtual device that appears when
        Zoom is capturing the screen with broadcast of the PC's sound?

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


