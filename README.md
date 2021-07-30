# OpenStartracker
An open-source 3D-printed startracker. Computer Vision + ML capabilities for automatic latitude calibration, polaris alignment, &amp; object tracking. 

<p align="center"><img src="https://github.com/adham-elarabawy/open-startracker/blob/main/media/animation.gif" alt="drawing" width="200"/><img src="https://github.com/adham-elarabawy/open-startracker/blob/main/media/startracker.png" alt="drawing" width="201"/></p>

**You can find my project page for OpenStartracker [on my portfolio website](https://www.adham-e.dev/project/openstartracker).**

## What is this?
OpenStartracker is a project dedicated to providing a lower-cost, open-source, machine-learning compatible solution to long-exposure astrophotography.

### How does it work?
Typically, long-exposure astrophotography solutions for DSLR camera (sold for >$300) work by rotating at exactly the speed of the earth's rotation about the polar axis. [This video](https://www.youtube.com/watch?v=WpmGi8DHu4c) explains the math behind this rotation very intuitively. However, in order for this rotation to properly compensate for earth's rotation, it has to first be aligned with the polar axis (about polaris), which is based on your latitude. 

This latitude alignment is usually _manually_ done via an equatorial mount, which just points the rotating base up at the north star. Given that latitude can be easily derived from gps location, I wanted to motorize + automate this latitude alignment as well using an iOS application + IMU sensor embedded in the design.

## Current Status
I am currently done with the mechanical design of the upper stage of the startracker, which is responsible for matching the speed of the earth's rotation to keep the stars in focus.

However, the lower stage of the startracker -- responsible for the automatic latitude adjustment -- has yet to be implemented (as well as the accompanying embedded IMU in the upper stage). 

With regards to electronics, they have all been tested and have been validated to work. 

With regards to software, the low-level motor control has already been implemented, but the iOS app interface has yet to be implemented.

To conclude:

- [x] Upper Stage Mechanical Design
- [ ] Lower Stage Mechanical Design
- [x] Electronics planning
- [x] Low-Level Motor Control Code
- [x] High-Level iOS application + bluetooth interface
- [ ] DSLR interface API
- [ ] CV polaris alignment functionality


## Mechanical Design
You can get access to the open-source mechanical design [via OnShape](https://cad.onshape.com/documents/eb5985eb85492b87b2d7116d/w/8a4f6561f5f12bc6eb17cdf7/e/3c6ea5c35ddcd26be48681a4), which I designed this project on.
