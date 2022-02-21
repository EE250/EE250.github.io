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

Ladder
- top is reference voltage, say 5V
- bottom is ground
- all resistances are the same here, so voltage is in even steps
- compare these to the input voltage

Triangles are Op Amps
- amplify differences in voltage
- if higher, on, if lower, off
- ask an EE major! (not Elijah)

Then use combinational logic to output bits

---



---

### Image Sources

https://wiki.analog.com/_media/university/courses/electronics/text/chptr20-f1.gif

https://microcontrollerslab.com/flash-adc-working-3-bit-example-advantages-applications/