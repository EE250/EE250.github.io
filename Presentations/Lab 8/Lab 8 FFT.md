class: middle, center

# Lab 8
### Fast Fourier Transform

???

Welcome all!
This week you'll learn to use the Fast Fourier Transform to analyze signals.

---

### Contents
- What is a Fourier series / transform?
- What do we use it for?
    - Advantages
- Lab Tasks

---

### Fourier
Series: Composes circles into a shape
Transform: breaks shape into circles
Sin / Cos: projections of a circle

???

To start, let's watch [a video](https://youtube.com/watch?v=r6sGWTCMz2k&t=0s).
- We see a bunch of arrows drawing a shape.
- Follow a single arrow, we see it rotates at a constant rate, tracing a circle
- By adding together a bunch of circles, we can get almost any shape – this is a Fourier series.

Of course, the shape is not and choice of circles is not an accident. 
We started with the shape, and calculated the Fourier series to make it.
The math behind that is beyond the scope of this lab.

Conceptually, that's what you need to understand:
- fourier series adds circles to make a shape
- fourier transform tells us, given a shape, what the fourier series is
    - it decomposes a shape into circles

---



- https://youtu.be/r6sGWTCMz2k?t=521
We can add sine waves together to create almost any waveform.
Here are some really beautiful illustrations: https://www.youtube.com/watch?v=r6sGWTCMz2k
- Notice how, even for shapes that are very NOT circular, and lines that are very NOT wavy, we can make them, out of sine waves.
- There's a lot of math we're going to step over here, and simply say:
- The fourier transform takes a wave, and decomposes it into a bunch of sine waves.

---

<div style="width: 100%; height: 100%; background-image: url(./Fig-1.png);background-repeat: no-repeat; background-size: contain;"></div>

???

From an engineering perspective, how can we use the Fourier transform?

We can use it to get information from a continuous wave.
- specifically, we're going to treat the amplitudes and frequencies as information.
- this is similar to, but different from the level based information in Lab 7.
  - With ADCs, we're capturing the level (e.g. of voltage)
  - With the FFT, we're capturing the frequency (e.g. of a sine wave)

So, what is the advantage of a different approach?

---

<div style="width: 100%; height: 100%; background-image: url(./Fig-1.png);background-repeat: no-repeat; background-size: contain;"></div>

???

To encode numbers when phone dialing. (e.g. Press 1 for more information)

\[Play sample audio here.\]

You may be able to make out the notes, as well as some noise.
- Noise might mess with a level based signalling system (e.g. if you tried to pass numbers by voltage level). 
- frequncy based systems are resilient to this kind of noise.
    - but e.g. police sirens might mess it up.

---

### Task

???

Visualize the FFT.

Then computationally use the FFT.

Note: you will have 2 peaks! You will need to figure out how to split them. 

---

# Fin.

???

Notes:
- [Illustration of composing 2 circles](https://jackschaedler.github.io/circles-sines-signals/dft_frequency.html)