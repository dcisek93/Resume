---
layout: post
title: Hyperlocal Weather Collection & Analysis 
description: Time Series Analysis, Hardware/Software Integration, Internet of Things 
image: assets/images/picarduino.jpg
nav-menu: false
---

This project presents an approach to capturing and analyzing local weather data in real time, with the long term goal of understanding near-surface deviations in meteorological conditions on the micro-scale. We approach this problem with an integrated approach, focusing on both the hardware and software requirements inherent in building such a system. I used an Arduino microcontroller with an ESP8266 wifi shield as the core of the sensor platform, with various sensors configued to capture real-time data about temperature, moisture, humidity, dew point, pressure, and altitude data. Several challenges are discussed, including the development of the sensor platform, the conversion of data from analog to digital, and the storage of data in an Internet of Things (IoT)-optimized database for easy access and visualization. Our approach focuses heavily on solving the hardware and data engineering challenges associated with such a task, but we also lay the foundation for future analysis and prediction tasks, by utilizing emerging time series analysis algorithms and prediction methods to gain insight into the data.

Currently this project has met all my short-term goals and we'll be posting the results of it soon for initial inspection. However, just because these initial goals were met doesn't mean this project is complete. If anything, it highlighted just how much more work remains to be done on this topic. We overcame many problems to get to this point, including optimizing how often the platform collects data and automating its scheduling, figuring out how to switch the platform to a low power mode to conserve battery life between individual collections, and making the jump from a hard-wired serial connection to a wireless card for streaming data directly to a web-enabled database. On the analysis side, we examine the relative strengths and weaknesses of five different types of models against several key variables gathered during our data collection phase. During that time, we collected over 24,000 data points, which provides a fantastic initial source of data against which to test these various machine learning and time series prediction methods. Below, we include a quick overview of the general workflow followed both on the hardware side (left) and our analytic pipeline (right). 

{:refdef: style="text-align: center;"}
{: refdef}
![image1](/assets/images/Workflows.png)
