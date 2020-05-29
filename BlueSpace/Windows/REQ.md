Envelopes (windows) were manually edited to have zero crossings, which are required by the Sakonda engine because it uses the sah~ object (sample hold) to pass parameter changes in sync with the phasor~ ramp, avoiding artefacts and glitches completely. 

Drawback is that envelopes have to be manually edited, as a normal hamming or gauss window doesn't contain zero crossings. 

This method allows for greater flexibility in individual grain sound, though clicks can be heard switching between windows.
