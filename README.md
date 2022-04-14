# OscPocket VA Synth - Daisy Pod Port
Alright, this is the OscPocketD VASynth, created by Staffan Melin, ported to work on the Daisy Pod. The goal of this project is to make a full-featured virtual-analog synth run on a fairly inexpensive platform (the Pod). This is mostly a personal project that I hope to share with others. I want to share everything because:

A. Open-source is great and I strongly believe that sharing everything you make will benefit the creator and the user
and, B. I don't really know what I'm doing and I hope someone else will come in and make this better

If you just want to use this synth on you Daisy Pod, download the .bin file and flash it using the web programmer on electro-smith.com. Here are the basic instructions.

First, you will need a midi keyboard or some sort of midi source to make any sort of sound out of this. When you boot this bad-boy up, you will see one of the two LEDs on you Pod light up red. The other will stay unlit. These two LEDs represent the menu to change the perameters of your synth. When you push the first button on your Pod, the first LED will cycle through colors, which will represent different categories, and when you push the second button, the second LED will also cycle through various colors, which represent specific perameters that can be adjusted. Each time the colors of the LED change, the function of the two knobs also change. It's not the best system, but again, the whole point of this is to have a compact, cheap, and high quality digital synth.

CURRENT MAJOR MISSING FUNCTION: I can't figure out how to save current settings/patches to be loaded again in the future. So that means when you power off your Pod, all settings will be lost. Thats a bummer I know, and I'm working on it/asking other people to help me out.

Here are what the colors mean and what perameters you can adjust:

<b><h1>Category 1: Red: Oscillators</b></h1>

RED/UNLIT
Knob1: Oscillator 1 waveshape
Knob2: Oscillator 1 level

RED/RED
Knob1: Oscillator 2 waveshape
Knob2: Oscillator 2 detune // this is not working exactly right. All the way counter-clockwise will detune second oscillator out of existance. But if you turn it past noon toward the right, you can get some more usable range.

RED/GREEN

Knob1: Number of voices (1, 5, or 8) // I only have three options here at the moment because previously if you turned the knob too fast, the Daisy Seed would hang up
Knob2: Amount of portamento // This is a little wonky at the moment and can be a little sensitive, but you can still dial in some nice portamento effect. Best used with just one voice

RED/BLUE
Knob1: Transpose Osc2 (Down 1 octave, no transpose, up 1 octave) 
Knob2: level of Osc2

RED/AQUA
Knob1: Pitch Envelope Attack
Knob2: Pitch Envelope Release

RED/PURPLE
Knob1: Pitch Envelope Decay
Knob2: Pitch Envelope Sustain

<h1>Category 2: Green: Amp Envelope</h1>

GREEN/UNLIT
Knob1: Attack
Knob2: Release

GREEN/RED
Knob1: Decay
Knob2: Sustain

GREEN/GREEN
Knob1: Noise
Knob2: Pan

<h1>Category 3: Blue: LFO</h1>

BLUE/UNLIT
Knob1: LFO Amount/Intensity
Knob2: LFO Frequency

BLUE/RED
Knob1: LFO Shape
Knob2: LFO Target: None, Pitch, Filter, Amp EG // to-do, I've been working on adding an option to target the Pan, but I haven't finished it yet

<h1>Category 4: Aqua: Filter</h1>

AQUA/UNLIT
Knob1: Filter Frequency
Knob2: Resonance

AQUA/RED
Knob1: Filter Envelope Attack
Knob2: Filter Envelope Release

AQUA/GREEN
Knob1: Filter Envelope Decay
Knob2: Filter Envelope Sustain //to-do, I want an option so you can set the filter envelope to match the amp evenlope

AQUA/BLUE
Knob1: Filter Type: in order CCW to CW: Low pass, high pass, band pass, notch, and peak
Knob2: Filter amount/Intensity // I may need to tweak this a bit, but I think it is giving the desired result of attenuating the filter envelope


<h1>Category 5: Purple: FX</h1>

PURPLE/UNLIT
Knob1: Delay Volume
Knob2: Reverb Volume // The volume of the reverb can only go as "loud" as the current wet setting. These two controls are meant to be quick access to tweaking the amount of FX after you have locked in the other settings. 

PURPLE/RED
Knob1: Delay time
Knob2: Delay Feedback

PURPLE/GREEN
Knob1: Reverb Filter
Knob2: Reverb Feedback

PURPLE/BLUE
Knob1: Dry signal amount
Knob2: Wet signal amount
