# MaxMSP-Experiments
  ## Blue Space
Live granular synthesis (GS) engine based on the [Sakonda Granular Synthesis v2.5 patch](http://formantbros.jp/sako/download.html). Features live looping and recording functionality, mouse driven sample scrub and random positioning system for evolving textures.

Definition of GS from Curtis Roads – "Granular synthesis deals with sound at a 'quantum' level: the sonic atom being the individual sample (any one of the 44100 taken in a second at the standard sampling rate)." 

The engine applies this concept by taking position information from a sample or live input, adding noise to the position and multiplying it by a certain duration in ms to create a 'grain' of the sample. 8 grains are played simultaneously with different phases, which creates a 'freeze' of that point – an eternal loop of that sample position. To control this, MIDI can be used to skip through the sample, or the repositioning system can scrub through randomly at a determinable rate.

  ## Entropy Cleric
Basic additive synthesizer with wave shape, ADSR, filter, LFO and overdrive controls. Includes a generative MIDI system based on selectable MIDI input that is used to make chords, in addition to a playable MIDI system. This was used to create the track 'Pareidolia' which is available on Soundcloud. Twitch Chat Integration was established using 'Chatty' Java app, though it is not automated as Max is unable to read from dynamically updated text files without manually reloading.
