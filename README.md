# MaxMSP-Experiments
  ## Blue Space
Live granular synthesis (GS) engine based on the [Sakonda Granular Synthesis v2.5 patch](http://formantbros.jp/sako/download.html). Features live looping and recording functionality, mouse driven sample scrub and random positioning system for evolving textures.

Definition of GS from Curtis Roads – "Granular synthesis deals with sound at a 'quantum' level: the sonic atom being the individual sample (any one of the 44100 taken in a second at the standard sampling rate)." 

The engine applies this concept by taking position information from a sample or live input, adding noise to the position and multiplying it by a certain duration in ms to create a 'grain' of the sample. 8 grains are played simultaneously with different phases, which creates a 'freeze' of that point – an eternal loop of that sample position. To control this, MIDI can be used to skip through the sample, or the repositioning system can scrub through randomly at a determinable rate.

![alt text](https://raw.githubusercontent.com/haelyons/Website-Content/master/BLUE%20SPACE.png)


  ## Entropy Cleric
Additive synthesizer with wave shape, ADSR, filter, LFO and overdrive controls. Includes a generative MIDI system based on selectable MIDI input that is used to make chords, in addition to a playable MIDI system. This was used to create the track 'Pareidolia' which is available on Soundcloud. Twitch Chat Integration was established using 'Chatty' Java app, though it is not automated as Max is unable to read from dynamically updated text files without manually reloading.

![alt text](https://github.com/haelyons/Website-Content/blob/master/ENTROPY%20CLERIC%202.png)

Instructions – from Max patch;
1. Ensure audio is turned on and master gain slider is above -inf.
2. Enable preferred oscillators – OSC1, OSC2, or Overtones –  and choose waveform. Ensure chosen oscillator gain is above minimum.
3. Change to preferred filter type or Bypass mode. 
4. Select input type:
     * If midi keyboard, ensure Spicey™ Generation toggle is off
     * If Spicey™, turn toggle on and modify parameters. 
5. Press preset 1, or another preset, and add notes to Spicey™ Generator if using instead of MIDI input (don't forget to toggle).
