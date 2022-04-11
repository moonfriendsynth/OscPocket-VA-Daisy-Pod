# moonfriendsynth
Alright, this is the OscPocketD VASynth, created by Staffan Melin, ported to work on the Daisy Pod. The goal of this project is to make a full-featured virtual-analog synth run on a fairly inexpensive platform (the Pod). This is mostly a personal project that I hope to share with others. I want to share everything because:

A. Open-source is great and I strongly believe that sharing everything you make will benefit the creator and the user
and B. I don't really know what I'm doing and I hope someone else will come in and make this better

If you just want to use this synth on you Daisy Pod, download the .bin file and flash it using the web programmer on electro-smith.com. Here are the basic instructions.

First, you will need a midi keyboard or some sort of midi source to make any sort of sound out of this. When you boot this bad-boy up, you will see one of the two LEDs on you Pod light up red. The other will stay unlit. These two LEDs represent the menu to change the perameters of your synth. When you push the first button on your Pod, the first LED will cycle through colors, which will represent different categories, and when you push the second button, the second LED will also cycle through various colors, which represent specific perameters that can be adjusted. Each time the colors of the LED change, the function of the two knobs also change. It's not the best system, but again, the whole point of this is to have a compact, cheap, and high quality digital synth.

CURRENT MAJOR MISSING FUNCTION: I can't figure out how to save current settings/patches to be loaded again in the future. So that means when you power off your Pod, all settings will be lost. Thats a bummer I know, and I'm working on it/asking other people to help me out.

Here are what the colors mean and what perameters you can adjust:

Category 1: Red: Oscillators

RED/UNLIT
Knob1: Oscillator 1 waveshape
Knob2: Oscillator 1 level

RED/RED
Knob1: Oscillator 2 waveshape
Knob2: Oscillator 2 detune

RED/GREEN

Knob1: Number of voices (1, 5, or 8)
Knob2: Amount of portamento //not working right now

RED/BLUE
Knob1: Transpose Osc2 (Down 1 octave, no transpose, up 1 octave)
Knob2: level of Osc2

RED/AQUA
Knob1: Pitch Envelope Attack
Knob2: Pitch Envelope Release

RED/PURPLE
Knob1: Pitch Envelope Decay
Knob2: Pitch Envelope Sustain

Category 2: Blue: Amp Envelope
Category 3: Green: LFO
Category 4: Aqua: Filter
Category 5: Purple: FX
