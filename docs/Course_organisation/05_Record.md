# Recording a Zoom session

According to the Zoom documentation, Zoom broadcasts a session in 720p. 
This is however not the format used for recording on the computer.
When recording, the resolution of the primary display is used, not that of
the monitor that displays the screen that is being recorded.

Hence, on the Mac, if the laptop screen is used and is the primary display
(which is the default behaviour), the recording will be in 16x10 format
with a very high resolution: 2800x1750. This in turn causes problems
in postprocessing, as (a) the format is not 16x9 (though this turns out
to be fairly easy to compensate in Shotcut) and (b) the interpolating to
1080p is rather time-consuming, making rendering of the videos extremely
slow.

Solution:

-   Use an external monitor in 1920x1080, e.g., the ASUS portable displays, and

-   Make that one the primary display.

This does imply that some applications will open on that display, but it turns
out that this does not disturb the recording. Just go with the mouse to the bottom
until the macOS task bar appears and open Zoom via the icon to get the Zoom screen
back.

