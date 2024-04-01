# Context
Tools made in MaxMSP. Max is a visual programming language intended for signal processing, and is especially useful for real-time applications. Below you can find 3 synthesizers, of which Entropy Cleric has a generative (algorithmic) composition tool. I use these mostly in the context of interactive support for multimedia performance.

You can listen to a stochastic piece made with the Entropy Cleric synth here: [Pareidolia](https://soundcloud.com/0x0c/pareidolia). Examples with Lydian Bells available on request :) 

  ## Lydian Bells (ring buffer FM synth) -- courtesy of Tom Dean
Frequency modulation based synth with interesting wave-shaping, ring-buffer when in Sustain mode to allow continual evolution of textures, and ADSR for individual note control. Requires Max 8.2.0 for the ADSR UI, though there are plain fields that can be used if this interface doesn't work.

  ## Blue Space (granular synth)
Live granular synthesis (GS) engine based on the [Sakonda Granular Synthesis v2.5 patch](http://formantbros.jp/sako/download.html). Features live looping and recording functionality, mouse driven sample scrub and random positioning system for evolving textures.

Definition of GS from Curtis Roads – "Granular synthesis deals with sound at a 'quantum' level: the sonic atom being the individual sample (any one of the 44100 taken in a second at the standard sampling rate)."

The engine applies this concept by taking position information from a sample or live input, adding noise to the position and multiplying it by a certain duration to create a 'grain' of the sample. 8 grains are played simultaneously with different phases, which creates a 'freeze' of that point – an eternal loop of that sample position. To control this, MIDI can be used to skip through the sample, or the repositioning system can scrub through randomly at a determinable rate.

For technical details and full functionality please [see here](https://helioslyons.com/posts/blue-space/). 

![alt text](https://raw.githubusercontent.com/haelyons/Website-Content/master/BLUE%20SPACE.png)

  ## Entropy Cleric (synth with stochastic note system)
Additive synthesizer with wave shape, ADSR, filter, LFO and overdrive controls. Includes a generative MIDI system based on selectable MIDI input that is used to make chords, in addition to a playable MIDI system. This was used to create the track 'Pareidolia' which is available on Soundcloud. Twitch Chat Integration was established using 'Chatty' Java app, though it is not automated as Max is unable to read from dynamically updated text files without manually reloading. For details on the generative system used for notes, and the overall functionality of the synthesizer, please see [this blog post](https://helioslyons.com/posts/entropy-cleric/).

![alt text](https://github.com/haelyons/Website-Content/blob/master/ENTROPY%20CLERIC%202.png)

  ### Instructions;
1. Ensure audio is turned on and master gain slider is above -inf.
2. Enable preferred oscillators – OSC1, OSC2, or Overtones –  and choose waveform. Ensure chosen oscillator gain is above minimum.
3. Change to preferred filter type or Bypass mode. 
4. Select input type:
     * If midi keyboard, ensure Spicey™ Generation toggle is off
     * If Spicey™, turn toggle on and modify parameters. 
5. Press preset 1, or another preset, and add notes to Spicey™ Generator if using instead of MIDI input (don't forget to toggle).

## Amp Player (amplitude threshold video player)
Dynamically fetches the amplitude of the last N seconds of sound and calculates a threshold value. When the value is exceeded by the input sound, `bang` message is generated which triggers the next video in a Jitter playlist. The Jitter video playlist works best with short snippets of videos or gifs that loop if the threshold is not reached before the end of that clip. The delta of the actual amplitude and the threshold value applies video effects to the jitter output. Audio is intended to be taken in from external applications -- ex. used in a live context with Serato or RekordBox while mixing.

## Future Uploads
A few projects I need to get around to uploading (please send a DM to give me a kick if these sound interesting to you):
- IDMIIb - A Open-NI Mate tool for the Kinect that allows manually allocation of points within a given 3D space to act as sample triggers. 
- IDMII - A Open-NI Mate tool for the Kinect that implements the concept of 'Mapping by Demonstration', whereby sound-motion pairs are recorded, and can then be played by in real-time with motion capture and granular re-synthesis. [blog post here.](https://helioslyons.com/posts/idm-2/)
