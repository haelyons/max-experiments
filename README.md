# MaxMSP-Experiments
  ## Blue Space
Live granular synthesis (GS) engine based on the Sakonda Granular Synthesis v2.5 patch (http://formantbros.jp/sako/download.html). Features live looping and recording functionality, new sample scrub and random positioning system for evolving textures.

Definition of GS from Curtis Roads – "Granular synthesis deals with sound at a 'quantum' level: the sonic atom being the individual sample (any one of the 44100 taken in a second at the standard sampling rate)." This engine applies the concept by taking position information from a sample or live input, adding noise to the position and multiplying it by a certain duration in ms to create a 'grain'. 8 grains are played simultaneously with different phases, which creates a 'freeze' of that point – great for atmospherics and pads.

  ## Entropy Cleric
Basic additive synthesizer with wave shape, ADSR, filter, LFO and overdrive controls. Includes a generative MIDI system based on sustained notes (screen input, not MIDI-controller enabled). Twitch Chat Integration (pending full functionality), using 'Chatty' Java app.
