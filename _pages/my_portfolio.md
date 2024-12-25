---
layout: archive
title: "Portfolio"
permalink: /my_portfolio/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

# Research Projects
# Computer Science
## Polynomial Reduction
## Chebyshev Encryption Scheme

# Data Analysis
## Analysis
## Frequency Resolved Optical Gating (FROG)

## Second Development for Equipments in Lab
* RedPitaya
  * [RedPitaya](https://redpitaya.com/) is an open source equipment for signal acquisition with two 125MS/s (million samples per second) RF (Radio frequency) outputs and two 125MS/s RF inputs, with 50 MHz analog bandwidth and 14-bit ADC (Analog-to-digital converter) and DAC (Digital-to-analog converter). It has a 16k sample buffer, and a -1 to 1V range.
  * <img src="/images/redpitaya1.png" width="500">
  * It has various built-in options for decimation, allowing us to select the desired sample rate and buffer time length. However, due to the limited 16k ADC buffer, the sample rate and buffer time length are inversely proportional.
  * <img src="/images/redpitaya2.png" width="1000">
  * In real-world optical measurement, we want to increase both the precision and buffer time length. Furthermore, we want the signal acquisition to be continuous.
  * To address this, I programed to divide its 16k ADC buffer into two 8k ADC buffers. When I stores the data in the first part, RedPitaya acquires the data in the second part. Thus, at some balance point of sampling speed, continuous signal acquisition is realized. As a result, we can acquire whatever length of time we want.
  * For example, data obtained by group members reached a length of 7x10^6 points, which is much longer than the original 16k points.
  * <img src="/images/redpitaya7.png" width="1000">
  * Now, we have continuous signal acquisition, and a problem that comes out immediately is memory occupation. To reduce it, I stored the binary data from the ADC buffer directly, resulting in a decrease in memory to 1/8. The data size above is 12.5MB.

* NiMotion ModBus
  * We needed to scan materials to analyze their changes under specific conditions. By integrating the RedPitaya software with a stepping machine [NiMotion ModBus](https://www.nimotion.com/), I implemented automated scanning.
  * <img src="/images/redpitaya3.png" width="500">
  * <img src="/images/redpitaya6.png" width="500">
  
* Graphical User Interface
  * To provide easy accessibility for other lab members, I created a Graphical User Interface using wxWidgets.
  * <img src="/images/redpitaya4.png" width="500">
  * <img src="/images/redpitaya5.png" width="500">
  * The project successfully led to my co-authorship of a paper [here](https://pubs.acs.org/doi/10.1021/acsphotonics.2c01851).
  * You can find the [codes here](https://github.com/ChillingLiu/Software_Developement/tree/main/RedPitaya_NiMotionModBus_Controler).

# Courses Projects

# Extra-curriculum
## 3D Modeling
I made a simulation video for the experiment of the Second Harmonic Generation FROG (Mentioned above) using Blender.
* ![image](/images/3D1.png)
* ![image](/images/3D2.png)
* You can find the video in [YouTube](https://www.youtube.com/watch?v=lTuWKqOZrFo).

## Posters
The posters I made for fun and during my work in Students' Association using Photoshop and Illustrator.
* <img src="/images/poster_newyear.png" width="500">
* <img src="/images/poster_gtsa.png" width="500">
* ![image](/images/poster_party1.png)
* <img src="/images/poster_party2.png" width="500">
* <img src="/images/poster_singer0.png" width="500">
* <img src="/images/poster_singer1.png" width="500">
* <img src="/images/poster_singer2.png" width="500">
* <img src="/images/poster_singer3.png" width="500">
