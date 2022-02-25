class: middle, center

# Lab 8
### Fast Fourier Transform

---

class: middle, center
### What is a Fourier series?

???

https://www.youtube.com/watch?v=r6sGWTCMz2k

Sine waves are projections of circles (that is, they show one dimention of a rotation).
If we add up lots of circles. We can make beautiful things.
But, how do we take a beautiful thing and turn it into circles?

This is what the Fourier transform does. (with complicated math).

---

class: middle, center
### Why do we care?

???

From an engineering perspective, how can we use the Fourier transform?

We can use it to get information from a continuous wave.
(Similar to the ADC we used in Lab 7).

How is this different? 
- With ADCs, we're capturing the level (e.g. of voltage)
- With the FFT, we're capturing the frequency (e.g. of a sine wave)

---

### Where is this used?

???

To encode numbers when phone dialing. (e.g. Press 1 for more information)

Play sample audio here.

Note the white noise. 
- This might mess with a level based signalling system (e.g. if you tried to pass numbers by voltage level). 
- frequncy based systems are resilient to this kind of noise.
    - but e.g. police sirens might mess it up.

---

### Task

???

Visualize the FFT.

Then computationally use the FFT.

Note: you will have 2 peaks! You will need to figure out how to split them. 