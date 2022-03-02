class: middle, center

# Lab 8
### Fast Fourier Transform

---

class: middle, center
### What is a Fourier series?

???

Simply put, we can add sine waves together to create almost any waveform.
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