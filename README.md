# MaxMSP-Experiments
This repository contains two projects made during my time learning and creating with MaxMSP at the University of Leeds, as part of the Music, Multimedia and Electronics BSc. MaxMSP is a visual programming language intended for signal processing, and is especially useful for live experimentation with digital signals. 

The first project is a granular sampler -- Blue Space -- with a number of customisable parameters and a special design using 8 phase-shifted grains for a more complex output. 

The second is a synthesizer -- Entropy Cleric -- built from scratch with  custom distortion and delay modules, as well as a generative note system that I designed and had a lot of fun playing around with (check out the generative piece of music I made with it: [Pareidolia](https://soundcloud.com/0x0c/pareidolia)).

  ## Blue Space
Live granular synthesis (GS) engine based on the [Sakonda Granular Synthesis v2.5 patch](http://formantbros.jp/sako/download.html). Features live looping and recording functionality, mouse driven sample scrub and random positioning system for evolving textures.

Definition of GS from Curtis Roads – "Granular synthesis deals with sound at a 'quantum' level: the sonic atom being the individual sample (any one of the 44100 taken in a second at the standard sampling rate)."

The engine applies this concept by taking position information from a sample or live input, adding noise to the position and multiplying it by a certain duration to create a 'grain' of the sample. 8 grains are played simultaneously with different phases, which creates a 'freeze' of that point – an eternal loop of that sample position. To control this, MIDI can be used to skip through the sample, or the repositioning system can scrub through randomly at a determinable rate.

For technical details and full functionality please [see here](https://helioslyons.com/posts/blue-space/). 

![alt text](https://raw.githubusercontent.com/haelyons/Website-Content/master/BLUE%20SPACE.png)

  ## Entropy Cleric
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

  ## Future Uploads
A few projects I need to get around to uploading (please send a DM to give me a kick if these sound interesting to you):
- IDMIIb - A Open-NI Mate tool for the Kinect that allows manually allocation of points within a given 3D space to act as sample triggers. 
- IDMII - A Open-NI Mate tool for the Kinect that implements the concept of 'Mapping by Demonstration', whereby sound-motion pairs are recorded, and can then be played by in real-time with motion capture and granular re-synthesis. [blog post here.](https://helioslyons.com/posts/idm-2/)
- A live VJ tool that takes a selection of images and performs some interpolation and beat matching (integrated with Serato DJ for live events). Just a bit of fun :)
