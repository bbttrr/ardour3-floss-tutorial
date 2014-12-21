Ardour: Recording

Recording Audio
===============

Besides Importing Audio, another way to create Regions in your Ardour
session is to record new audio. The source of this audio could be the
line or microphone inputs of your audio interface, or it could even be
sound originating from other applications on your computer which have
been connected to Ardour via JACK. Please see the section on **Routing**
for more details.

This section will show you how to record audio from an external source
(for example, a microphone) onto a track in Ardour.

First, you should check that the proper inputs have been routed to the
track you wish to record to. Select the track by clicking on the empty
space just below its name and volume slider. The Track becomes
highlighted. The vertical strip **Editor Mixer** located on the left
side of the Editor window should now show the Track you just selected
(*Audio 1* in this example). If you don't see the Editor Mixer strip,
use the shortcut "*Ctrl*" + "*E*" to make it appear. Just below the
Track name in the Editor Mixer you will find a button that allows you to
edit the Routing. Click on that button to investigate the Routing.

![](static/Ardour3_Editor_Mixer_Input_1.png) \

In the image below you can see that the only input of this Mono Track is
receiving signal from *system capture\_1*. This normally means the first
microphone input of your soundcard. \

![](static/Ardour3_Audio_1_input.png) 

The tabs that you see displayed vertically on the left are available
sources. "*Audio 1 in*" that you see on the bottom right is the
destination. The green dot represents a connection.

The **Ardour** tabs show the connections that can be made from other
sources within Ardour. The **Other** tab displays audio connections
available from software other than Ardour. The **Hardware** tab shows
hardware connections (for example, the built-in microphone of your
computer or the inputs from your sound card). In all cases, this Routing
matrix communicates directly with JACK to change the Routing in the JACK
system itself. This will be explained in more detail in the
**Understanding Routing** chapter. 

For the purpose of this chapter, simply make sure that system capture\_1
(from Hardware tab) is connected to the Audio 1 track so that we can do
a test recording. If you don't see a green dot as in the screenshot
above, click on the matrix to make the connection manually. You can now
close this window.

*Note: the example above assumes you are recording a Mono sound source
onto a Mono Track. If you want to record in Stereo, the instructions are
pretty much the same, but you should create a Stereo Track and you will
see two green dots, one for capture\_1 and another for capture\_2.*

### Arming the Track

"Arming the Track" is simply to get it ready for recording. Once you
have checked that the proper capture inputs have been routed to the
Track, you can arm the Track to record by clicking on the small red icon
on the horizontal track strip (not the big one in the Transport
controls). When properly armed, the small red icon will remain
highlighted, and you will be able to see the incoming signal by looking
at the **Peak** **Meter** on the Editor Mixer or on the horizontal Track
strip.

*Note: unless you have told Ardour to do otherwise, the input being
recorded will be monitored (in other words, heard) via
the***Audition***output. If you are not using headphones to monitor the
recording process, you may get some loud feedback at this point!*

### Arm Ardour and Start Recording

Now that you have armed the Track to record, you must arm Ardour itself
to record by clicking on the big red button in the **Transport menu**.
The button will blink in red, indicating that Ardour is ready to record.
To start recording, click on the Play button in the Transport menu, or
press the space bar of your computer keyboard. Clicking the Play button
again (or pressing the space bar) will stop recording.

![](static/Ardour3_Recording.png) \

While recording, the armed Track will capture the sounds from the input.
Any existing sound on other tracks will play normally during the
recording. This allows you to play, sing or speak along with other
Regions and Tracks you have already recorded or embedded in your
Session.

While recording, you will be able to see the **Levels** (the amplitude
in Decibels) of the incoming sound, as well as see the **Peaks** of the
**Waveform** appearing as it is recorded.

The audio in the screenshot below was recorded too loud and produced
**Clipping** (in other words, the signal recorded was outside the bounds
of what could be represented digitally), which results in a loss of
information and audible distortion. The clipped peaks in the waveform
are marked in red, and the **Peak Meter** in the Editor Mixer strip has
registered a maximum signal level of 1.0 Decibels over the limit of zero
Decibels.

![](static/Ardour3_Clipping.png) \

The best and easiest way to avoid Clipping is have some control over the
volume of the incoming audio signal before it gets to the sound card.
For example, you can can move the microphone further away from the sound
being recorded or use a mixer to reduce the volume of the incoming
signal. 

When the audio signal has been recorded within proper limits, you should
see no red Peaks, and the level meter should show a negative number as
maximum peak (for example, a maximum peak of around −3.0 Decibels allows
for a comfortable distance from the Clipping Point.)

The range of decibels between the region's maximum Peak and the Clipping
Point is commonly referred to as **Headroom**. It is common recording
practice to keep approximately three to six Decibels of Headroom between
the maximum of your signal and the Clipping Point, with the Clipping
Point itself being represented as 0dB (zero Decibels). In other words,
an audio region with a comfortable amount of Headroom would have its
maximum Peaks between −6dB and −3dB.

Recorded audio appears as a new Region in the recording Track. Like all
Regions, this newly recorded one will be available in the Region List,
from where you can drag-and-drop it into other Tracks if needed.

The Region you just recorded will automatically receive the name of the
Track where it was recorded, with different takes being automatically
numbered. In the screenshot below, "*Audio 1-1*" and "*Audio 1-2*"
represent two different recordings made on a track named "*Audio 1*". \

![](static/Ardour3_RegionList_Recording.png)

You might want to plan ahead and organize your recording Session by
giving appropriate names to different tracks. For example, a Track used
only for recording vocals can be named "Voice". This way, recorded sound
files will be named accordingly, and different takes will appear in the
Regions List identified as "Voice-1", "Voice-2", etc, rather than the
default generic names, such as "Audio 1".

To rename a Track, just click on its name (before you arm the track to
record) and type in the new name.

Continuing
----------

At this point, you may want to skip directly ahead to the **Editing
Sessions** section to learn how to arrange the Regions you have Recorded
into a composition. If you plan on doing more complicated Recording than
what we have discussed here, in particular with a multichannel
soundcard, or from other JACK-enabled audio programs on your computer,
you should also have a look at the **Understanding Routing** chapter.
