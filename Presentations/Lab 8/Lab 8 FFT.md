class: middle, center

# Lab 8
### Fast Fourier Transform

???

Welcome all!
This week you'll use the Fast Fourier Transform to analyze signals.

---

### Contents
- What is a Fourier series / transform?
- What do we use it for?
    - Advantages
- Lab Tasks

---

class: middle, center

# Fourier Series
### Composes circles into a shape

# Fourier Transform
### Decomposes shape into circles

???

Conceptually:
- fourier series is a set of circles that compose a shape
- fourier transform tells us, given a shape, what the fourier series is
    - it decomposes a shape into circles

[Demonstration](https://youtube.com/watch?v=r6sGWTCMz2k&t=0s)
- We see a bunch of arrows drawing a shape.
- Focus on one arrow. It rotates at a constant rate, tracing a circle
- By composing circles, we get a shape 
    – this is a Fourier series.

The shape and choice of circles is not an accident. 
Starting with the shape, we used the Fourier transform to derive the series.

The method (and math) is beyond the scope of this class.
- EE students may encounter it.

(Reiterate Concepts)

---

class: middle, center

# Waves
### Periodic Movement In Space

???

Can someone give me an example of an IRL wave?
- Sea waves? - these are sinusoidal
- waves don't have to be!
- wave = periodic movement in space
    - square wave, sawtooth wave, triangle wave, etc.

Point: 
- this is a 2D wave
- shape is drawn periodically
- fourier transform breaks 2D waves into circles

---

class: middle, center

# Sin / Cos
### [Projections of a circle](https://jackschaedler.github.io/circles-sines-signals/sincos.html)

???

[Wave Demo](https://youtu.be/r6sGWTCMz2k?t=521)

The 1D Fourier Transform
- We start with circles, they're pretty!
- usually, you'll encounter 1D waves, broken into sinusoids
- point: this is the same, simply projected!
- Recall sin/cos are just projections
    - that is, they look at 1 dimension of a 2D rotation

---

class: middle, center

# Questions!

---

class: middle, center
# Fourier Transform & Information
### Phase
### Amplitude
### Frequency

???

Return to the music note.
- It "contain"s the circles, we "extract" them with the Fourier transform
- Circles hold information: phase, amplitude, frequency
- Transmitting the wave is like transmitting all information in the circles

Similarly, a 1D wave contains a range of frequencies at different amplitudes.
- engineer speak for: Music!

Your ears are a great signal analysis tool for music.
- (Play Sample Here)
- you can hear the notes – that's information!

---

<div style="width: 100%; height: 100%; background-image: url(./Fig-1.png);background-repeat: no-repeat; background-size: contain;"></div>

???

What that looks like
- this is a lab 8 screenshot
- let's break the plot down

Top Left
- Time plot
- Wave density due to high frequency

Top Right
- Slice of the time plot, focusing on the first section
- Wave is clearer

Bottom
- Frequency plot – result of the Fourier transform
- see 2 notes

---

<div style="width: 100%; height: 100%; background-image: url(./Fig-2.png);background-repeat: no-repeat; background-size: contain;"></div>

???

- So, what information does this encode?
- One digit in a phone number!

- To encode numbers when phone dialing. 
    - (e.g. Press 1 for more information)

---

# Tasks
### Create Plots
### Find Number
### Find it Programmatically

???

Tasks: 
- Visualize the FFT.
- Then computationally use the FFT.

---

class: middle, center

# Noise

???

(Play Noisy Sample 3)
- Resilient to white noise, which might mess up a level based system
- However, narrow interference is still a problem
    - e.g. police siren.

---

# Fin.

???

Notes:
- [Illustration of composing 2 circles](https://jackschaedler.github.io/circles-sines-signals/dft_frequency.html)

One cool thing: 
- using circles to make **not** circular shapes
- even a "sharp" corner! 

Detail: all circles use discrete frequencies
    - i.e circle 2 rotates 2x as fast as circle 1