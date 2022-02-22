class: middle, center

# Lab 7
### Analog-Digital Conversion

---

# Contents

1. Motivation
2. Analog-Digital Conversion
3. Digital-Analog Conversion

???

- Goal: gain understanding of analog-digital conversions
- First, has this been covered in lecture?

- You'll be implementing 2 virtual circuits to perform these functions

---

# Motivation

<div style="width: 100%; height: 100%; background-image: url(./ADC.gif);background-repeat: no-repeat; background-size: contain;"></div>

???

Analog: 
- continuous in quantity (voltage)
- continuous in time

Digital: 
- discrete in quantity (few bits)
- discrete in time

Our strategy: sample the analog periodically, to create a digital signal.

That leaves the question: given some voltage at some instant in time, how do we get bits out of it?

---

<div style="width: 100%; height: 100%; background-image: url(./Flash-ADC.jpg);background-repeat: no-repeat; background-size: contain;"></div>

???

- Flash ADC
- uses a "ladder" of resistors
    - so called because voltage gets higher as you go up

Ladder (on the left)
- at the top is a reference voltage, say 5V
- bottom is ground
- we assume our analog signal falls between this voltage range
- all resistances (R) are the same here, so voltage is in even steps (V1-V7)
- next step: compare these to the input voltage

Triangles are Op Amps
- amplify differences in voltage
- if the top voltage is higher, they "turn on", if lower, off
- ask an EE major! (not Elijah)
- the important part: we can treat their output as binary

Last step: Then use combinational logic to encode into a binary number
- you need to figure this out

---

class: middle, center

# ADC Questions?

???

Questions.

Lets move onto Digital-Analog Conversion.

---

<div style="width: 100%; height: 100%; background-image: url(./DAC.png);background-repeat: no-repeat; background-size: contain;"></div>

???

Digital to analog converters are a harder.
The diagram and equations help, but please do ask us for further explanation.

If you go through the equations on the page, you'll find the output voltage is negative.

Your last task is to invert the voltage so that it is the same magnitude, but positive. (Hint: use an inverting Op Amp)

---

### Image Sources

https://wiki.analog.com/_media/university/courses/electronics/text/chptr20-f1.gif

https://microcontrollerslab.com/flash-adc-working-3-bit-example-advantages-applications/

https://www.electronics-tutorial.net/analog-integrated-circuits/data-converters/binary-weighted-resistor-dac/