# march notes


## understanding ground and voltage

Trying to understand what
50 ohms impedance in coaxial and as well as dipoles actually means. Rather than just a diagram or someone telling me the facts and that the dipole ranges from 0 in the middle to infinity at the end

What is happening in the coax

A couple explanations - from chat gpt  the L and C are distributed throughout the cable so there is no reactance (Different but related question)

https://youtu.be/RkAF3X6cJa4?si=WhM9E53WBnwUlpox

This post treats the resistance like essentially a replacement value for how the electrons behave, with an “expectation of 50ohs” given the properties of ohms law and the cable
Replace a fake resistor 

Last night discussion on j antenna and how the quarter wave matches the impedance of the infinite side of the dipole 

I might just be looking too far ahead in the book

Do t confuse the 50ohms with dc it’s ac 
Don’t think of it as how hard is it to push elections through something

It’s how hard is it to CHANGE the v and a 


So the impedance is really:

The ratio of magnetic energy storage to electric energy storage along the cable.

For a given voltage wave, how much current wave exists with it.

Based on the constructed geometry of the cable and how much l and c it has

More of a design feature. Not a loss the same way like a “bad” thing

Stuck in dc, resistor as something to push thinking rather than the more advanced sine wave

The Deeper Truth

Impedance is not “a thing” like a resistor.

It’s:

The relationship between voltage and current in a system where energy is oscillating between electric and magnetic fields.

That’s it.

And the moment you understand that, 50 Ω stops being a magic number and starts being a design compromise between:
	•	Power handling
	•	Loss
	•	Mechanical size

(Which is why 50 Ω became standard in RF systems.)

Voltage ground 


## Working on Astable Multivibrator 
Goals: 
- Understanding why resistors are needed before each component
- Understanding flow of electricity during each step, solidify knowledge of behavior of transistors, caps, resistors, LEDs
- Reading resistor color codes
- Wiring on a breadboard 

### Components
Resistors used - 
-2 100k ohms to collectors 
-2 10k ohms to base / capacitors 

- 2 100 microfarad caps
- 2 LEDs
- 2 2n2222 NPN transistors

Vcc = 5V


### Why ~0.6V Matters

Silicon BJT base-emitter junction behaves like a diode.
Needs ~0.6–0.7V to conduct.
That threshold determines switching timing.
If you ever see ~0.6V and wonder why — it’s physics, not magic.

### Base Resistors (e.g., 10kΩ)

Limit base current.
Set charge rate of capacitor.
Help determine oscillation period.
LED Resistors (e.g., 470Ω)
Limit LED current.
Protect LED and transistor.
Set brightness.

## Timing formula
For symmetric design:

T≈1.4×R×C
T≈1.4×R×C

Where:

R = base resistor

C = capacitor

It took me a little while to figure out how to wire correctly, basically treating the entire top of the circuit board as a + and the entire bottom as the negative with a cord linked. 

The other item was understanding why the current would go through the open transistor instead of through the LED, it's becaues of less resistance. Was able to walk through the circuit and understand each step and what ishappening. 

Think this through - why does when side have 100 micro farads and the other 10, the 100 microfarad connected to the base of the transistor, the led connected to the 10 mf blinks and the other does nothing 

It's staying closed so long that the smaller cap has a long time to charge, so even when teh other light goes off, it wont' go on because it had so much time to charge. 
