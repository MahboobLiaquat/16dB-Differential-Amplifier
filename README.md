6 dB Differential Amplifier

This project features a custom-built, two-stage differential amplifier designed to amplify weak differential signals while rejecting high-frequency common-mode displacement current. It is ideal for use in experimental setups such as Time-of-Flight and Interrupted Field Time-of-Flight measurement techniques, where rejecting common mode signal and amplifying the weak photocurrent signals from samples such as Amorphous Selenium are critical.

## Overview

The amplifier consists of two stages:
1. **Stage 1: Unity-Gain Differential Amplifier (AD830ARZ)**
   - High-CMRR, wide-bandwidth video amplifier from Analog Devices
   - Unity-gain configuration with a CMRR of 60 dB at 4 MHz
   - Bandwidth: 85 MHz
   - Isolates common-mode noise from the input signal

2. **Stage 2: Non-Inverting Amplifier with Gain of 16 dB (AD827)**
   - High-speed operational amplifier from Analog Devices
   - Gain configured via feedback resistor selection (gain = 6.3×)
   - Amplifies the cleaned differential signal above oscilloscope base noise

Both stages are powered by ±15V. The amplifier is enclosed in a shielded box to minimize electromagnetic interference. 0.1 µF decoupling capacitors are used near the power supply pins for additional filtering.

## Features

- Differential signal amplification with 16 dB gain
- High noise rejection capability
- Optimized for fast transient response
- Powered by a symmetrical dual ±15V supply
- Shielded aluminum enclosure
- Easily connected via front-panel BNC jacks

## Usage Notes

- Inputs should be connected with proper BNC grabbers.
- Ensure common ground is shared across power supply, DUT, and oscilloscope.
- When probing output on oscilloscope, hook the signal after the 500 Ω resistor to ground.
- Incorrect grounding or unequal power rails may cause large offsets.
