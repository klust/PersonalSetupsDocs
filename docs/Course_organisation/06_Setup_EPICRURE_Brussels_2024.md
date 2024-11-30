# Setup for the EPICURE meeting in Brussels, 2024

The meeting took place at FWO, so the challenge was to make it possible to use
ClickShare.

## Materials

### Hardware

-   Screens:

    -   Both ASUS portable monitors and their cables.

-   Microphone:

    -   DJI microphone set + included USB-D - USB-A cable

    -   Little tripod

-    Webcam
  
    -   LogiTech StreamCam HD + tripod attachement

    -   Lightweight tripod MEfoto backpacker air

    -   USB-C extension cable (male to female)

-   Video capture:

    -   Elgato HD60X + its included USB-C - to - SUB-A cable + its included HDMI cable 
        (the latter too short for the room though)

    -   6m HDMI cable

-   iPad to steer the presentation

-   Other hardware:

    -   Logitech Presenter

    -   Logitech Pebble

    -   Docking station OWC Thunderbolt Go Dock

    -   USB power supply with cable for charging the microphone charging case and cable for the iPad

    -   Power distribution block


### Software

-   OBS Studio

-   OBS Blade on the iPad

-   Zoom

-   VB-Cable A+B package

-   Audio Hijack


## Setup

### Hardware

-   Portable monitors:
  
    -   ASUS USB-C monitor to the left of the laptop, lined to second TB port on 
        the dockingstation counting from the left.

        Presentations can be done from this screen and are captured via OBS.

    -   ASUS HDMI monitor to the right of the laptop. This screen is a copy of what will
        be shared through ClickShare. Connected to the left TB port on the back of the 
        docking station.

-   Microphone receiver on tripod, connected with USB-C - to - USB-A to USB-A port on
    the back of the docking station.

-   Webcam on MEfoto tripod, USB-C elongation cable plugged directly into the laptop
    as the image was not stable when in the docking station. 

-   HD60X capture device with 

    -   USB-C - USB-A cable to port on the rear of the docking station.

    -   Long HDMI cable to the presenters' table

-   LoupeDeck CT with the included USB-C cable and USB-C -to -USB-A adapter to the 
    front (USB2) port of the docking station.

-   iPad + Airpods for monitoring or for OBS Blade


### Software

-   macOS sound:

    -   Output to whatever is available in the room

    -   Input to whatever, e.g., Wireless Microphone RX

-   Zoom setup:

    -   Connect camera to "OBS Virtual Camera"

    -   Speaker to VB-Cable B

    -   Microphone to VB-Cable A

    -   Music profile for sound with echo cancellation though that may not be needed
  
    -   Make sure that the camera is on in the meeting and that the speaker is not 
        muted.

-   Audio Hijack setup

    -   Check how you can get sound in the room

    -   Session: Send sound from HD60X to the room to hear the sound of the 
        presenters' laptop

    -   Session: Send sound from VB-Cable B to the room to hear Zoom conversations

    -   Session: VU meters on VB-Cable A to check if there is sound going to Zoom.

-   OBS setup:

    -   Use the EPICURE 2024 scene collection

    -   Device connections:

        -   **Video HD60X** and **sound HD60X** to the HD60X

        -   **CAM** and **Audio CAM** to "Logitech Streamcam"

        -   **LTP scr cap** aan de "ASUS MB166C"
    
    -   Global audio devices in the "Settings" in the right dock:

        -   **Mic/Aux** to *Default settings*

        -   **Mic/Aux 2** to * Wireless Microphone RX**

        -   **Mic/Aux3** to *Game Capture HD60 X*

        -   **Mic/Aux 4** to *VB-Cable B*

    -   "Advanced Audio Properties" in the Audio mixer (from the "All sources scene"):
        All are monitor and output, except "Zoom (B)" which is "not monitor" as we don't want to
        feed that back into Zoom.

    -   Use "Tools"-> "Websocket settings" to enable websockets so that "OBS Blade" on the iPad can
        be used to steer scenes. This is essential when presenting from the laptop as PowerPoint needs
        to be in focus for that.

        Turn off authentication as the LoupeDeck software cannot authenticate, and there are 
        sometimes trouble to get the connection in OBS Blade on the iPad also.

    -   You can use the "preview" feature both at the "Sources" level or in the preview zone to send
        the output of the sources or of the preview zone to the second ASUS monitor which is then
        duplicated with ClickShare.

