---
layout: post
title: Hyperlocal Weather Collection & Analysis 
description: Time Series Analysis, Hardware/Software Integration, Internet of Things 
image: assets/images/picarduino.jpg
nav-menu: false
---

This project presents an approach to capturing and analyzing local weather data in real time, with the long term goal of understanding near-surface deviations in meteorological conditions on the micro-scale. We approach this problem with a two-fold perspective, focusing on both the hardware and software requirements inherent in building such a system. I used an Arduino microcontroller with an ESP8266 wifi shield as the core of the sensor platform, with various sensors configued to capture real-time data about temperature, moisture, humidity, dew point, pressure, and altitude data. Several challenges are discussed, including the development of the sensor platform, the conversion of data from analog to digital, and the storage of data in an Internet of Things (IoT)-optimized database for easy access and visualization. Our approach focuses heavily on solving the hardware and data engineering challenges associated with such a task, but we also lay the foundation for future analysis and prediction tasks, by utilizing emerging time series analysis algorithms and prediction methods to gain insight into the data. Towards this end, the relative strengths and weaknesses of five different types of machine learning and time series prediction models were tested and evaluated against several key variables gathered during the data collection phase.

This project meshed my personal interest in IoT development and real-time data collection with the requirements of The University of Missouri's Data Science & Analytics (DSAN) Graduate Certificate program. This project served as my capstone for this program, but also grew in scope to satisfy my own curiosity. Currently this project has met all my short-term goals, having collected a data set of over 30,000 data points for each sensor, cleaning and storing this data for future use, and building a complete time series analytics pipeline. Over the course of this project several major hurdles were overcome, including optimizing how often the platform collects data and automating its scheduling, figuring out how to switch the platform to a low power mode to conserve battery life between collections, and making the jump from a hard-wired serial connection to a wireless connection for streaming data directly to a web-enabled database. Below, we include a quick overview of the general workflow followed both on the hardware side (left) and our analytic pipeline (right). 

{:refdef: style="text-align: center;"}
{: refdef}
![image1](/assets/images/Workflows.png)

<br> 
<center>Here's a picture of the final platform, pictured here with the cover removed from its weather-proof housing. </center>

{:refdef: style="text-align: center;"}
{: refdef}
![image1](/assets/images/NoLid.jpg)
