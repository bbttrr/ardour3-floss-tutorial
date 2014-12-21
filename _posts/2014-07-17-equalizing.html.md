Equalizing
==========

Often, even after adjusting Levels and Panning, different tracks with
similar frequency content (for example, a bass guitar and a kick drum)
may be difficult to tell apart in the Mix. A good tool to address this
issue is an**Equalizer** (or **EQ**). Essentially, an equalizer allows
you to separately control the gain of different frequency ranges of a
sound. This can be useful not only to sculpt the timbre of an isolated
sound (for example, to make it sound 'sharper' or 'smoother'), but also
to make sounds of various timbres to integrate better into the Mix. \

3-Band Equalizer
----------------

The simplest kind of Equalizer is the one familiar to us from analog
mixers. It has three parameters, which adjust the Levels of three
**Bands**, or frequency ranges: one for the **Bass** (low frequencies),
one for the middle range frequencies and one for the **Treble** (high
frequencies). The "*DJ EQ*" LADSPA Plugin is just such an EQ.

![dj\_eq](static/Ardour-MixerStrip-dj_eq-en.png "dj_eq")

Multi-Band (or Graphical) Equalizer
-----------------------------------

A more complex **Multi-Band (or Graphical) Equalizer** often has between
eight and thirty-two Bands. Each Band is centered on a frequency, and
the Level of each Band can be independently adjusted. In some Multi-Band
EQs, such as the "*TAP Equalizer*" LADSPA Plugin shown below, the center
frequency of each Band can be defined by the user. This allows you to
either attenuate (or remove) an unwanted frequency, or to reinforce
(boost) a desired one.

![tap\_eq](static/Ardour-MixerStrip-tap_eq-en.png "tap_eq")

The overall "curve" of the Bands can also be used to determine the
general tone of your Track or Mix. In the example above, the lower part
of the mid-range frequencies have been "scooped out" a bit (note how
Bands 1 and 8 are left untouched at 0 dB, while intermediary Bands 2 to
7 draw an attenuation curve, with Band 4 at -13 dB as the lowest point).
\

Parametric Equalizer
--------------------

The **Parametric Equalizer** is the most versatile type of EQ used for
Mixing because of its extensive control over all types of EQ parameters.
In Ardour there is a Parametric Equalizer called the "*Triple Band
Parametric with Shelves*", located in the Plugin folder labeled "*Steve
Harris*".

![parametric\_eq.png](static/Ardour-MixerStrip-parametric_eq-en.png)

There are three options for each Frequency Band. Each of the three Bands
has a "*gain (dB)*" adjustment to cut or boost frequencies, a
"*frequency (Hz)*" adjustment to select center frequency, and a
"*bandwidth (octaves)*" slider which determines how wide the range of
frequencies to be affected will be. This plugin also contains a **High
Shelf** and **Low Shelf**. A **Shelf** cuts or boosts everything above
(High Shelf) or below (Low Shelf) a specific frequency. For example, a
Low Shelf can be used to remove unwanted rumbling sounds, and a High
Shelf can be used to reduce hiss.

An Example of Using an Equalizer
--------------------------------

In order to achieve a better separation of two instruments in the Mix
through the use of EQ, you first need to find out where the two
instruments overlap.

Here's one approach. In the *Triple Band Parametric with Shelves*
Plugin, select an appropriate Band for one of the instruments. In the
case of a bass guitar, it would be "*Band 1*", the low frequency band.
Boost the "*gain*" to 10dB, increase the "*bandwidth*" so that is a
narrower range up to 3, and then scroll the "*frequency*" up and down
slowly. You'll hear a pitch move up and down. Then scroll it down slowly
until you hear the frequency range where the two instruments overlap.
Now simply reduce the "*gain*" to -5dB, and you will hopefully hear the
instruments a bit clearer. Next, apply the same process to the other
instrument.

There are many approaches to EQ. Hopefully this will provide one example
of how to begin EQ'ing Tracks in your Mix. But most importantly, when it
comes to EQ, it is better to use too little than too much, unless you're
consciously using extreme EQ as a compositional parameter.

Continuing
----------

You should have enough tools now to create a clean, well-balanced Stereo
Mix of your Session. However, if you want the parameters of your Faders,
Panning or Plugins to change over Time, then you will want to explore
the **Using Automation** chapter next. If not, then skip ahead to learn
how to **Export Sessions** in the following section.
