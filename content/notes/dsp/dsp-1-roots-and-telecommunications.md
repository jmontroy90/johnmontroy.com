+++
date = "2023-09-25"
draft = false
tags = ["dsp"]
title = "DSP 1: Roots and Telecommunications"
+++

_(blog images will always be generated by some LLM or another, today Stable Diffusion)_

Covered: 

- _Chapter 1: _[The Roots of DSP](https://www.dspguide.com/ch1/1.htm)
- _Chapter 1: _[Telecommunications](https://www.dspguide.com/ch1/2.htm) 

Digital Signal Processing answers the question: “What do I do with all these data I just converted from analog to digital?” That can include a huge array of disciplines and industries. DSP used to be very specialized, to oil discovery or space exploration, but once personal computers hit the scene in the 80s, everyone had access to DSP. DSP is one of those fields like electronics - in today's world, everyone working in science or engineering probably should know at least a little bit about it!

### Telecommunications

Telecom companies need to pass customer information over some physical channel (fiber optic, radio, whatever). The better they can do it, the more money they make.

- **Multiplexing:** Before digital, analog signals had to be routed directly (“I’ll patch you through”), meaning one convo == one wire. Digital signals of bits can easily be multiplexed - the T-carrier can do 24 simultaneous signals sampled 8000 times / second with a bit depth of 8 bits, for a total of ~1.5MBits/second. These signals can be transported 6000 feet over standard telephone line 22-gauge copper wire.
- **Compression:** There are many ways to compress a signal without losing fidelity. Some use cases can compress all the way to 2kbps (like submarines), and up until 8kbps is pretty much fine.
- **Echo control**: signals bounce back, and we need DSP to generate anti-signals to cancel these echoes out. The ear will detect them if they’re longer than a few seconds!