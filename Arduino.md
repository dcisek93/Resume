---
layout: post
title: Local Weather Prediction with Arduino, Keras 
description: Time Series Analysis, Hardware/Software Integration, Deep Learning 
image: assets/images/picarduino.jpg
nav-menu: false
---

This project merged aspects of hardware and software development, to collect, analyze, and predict local weather changes over a short time window (six hours). I used an Arduino microcontroller with an ESP8266 wifi shield as a sensor platform, which I built and configured to collect real-time data about temperature, moisture, humidity, pressure, and altitude. I programmed it to wirelessly stream data to an Internet of Things (IoT)-optimized database, which provided an easy solution to store and visualize my data holdings. <br> <br>
Currently I'm in the process of optimizing how often it collects data, and how between individual collections we can switch to a low power mode to conserve power. From there I'll move forward with the analysis portion of the project, using several approaches to time series analysis and prediction, and plan to rely upon the Keras library to predict whether it will rain or not over the next six hours. 


{:refdef: style="text-align: center;"}
{: refdef}
![image1](/assets/images/glacier.png)
