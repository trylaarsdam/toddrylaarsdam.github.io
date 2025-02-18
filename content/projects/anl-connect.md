---
title: "ANL Connect"
description: Flutter, Kotlin, BLE, Particle MCUs, STM32 MCUs
date: 2021-10-25
author: 
  display_name: Windy City Lab/Argonne National Laboratory
---
Completed: 2021-10-25 | Client: Argonne National Laboratory | Employer: Windy City Lab

---

{{< imagewithtext img="/assets/anl-connect.jpg" >}}

ANL Connect controls and configures Gen3 Gemini series underground soil sensors built by Windy City Lab for Argonne National Labs. Currently the app is only available for Android, but there are plans to add iOS support in the future.

The app uses low energy bluetooth (BLE) to communicate with the testing devices. Since we want to make sure everything is working as expected during our testing, the protocol that the app uses to communicate over BLE is very robust and filled with confirmations. There are confirmations for the device receiving a message, what the message said, and that the action requested was executed. This allows us to make sure what we think is happening is actually happening. 

The app also ties into our database to show you realtime data from the devices, so you know instantly whether the transmission you just sent was received by the receiver or not. This allowed us to efficiently and confidently test the devices in the field, as we knew exactly what was or wasn't working, and we weren't questioning the results our tests were giving us.

## Making the project

This project was made over about 2 weeks, and was actually my first time ever writing an Android app or using the Kotlin language. For the UI I used Jetpack Compose, which seemed to be the right choice for new apps. The BLE scanning and connection part was a tad frusterating to get working, but I'm attributing that to my lack of experience with the language and the Android API. As I look back at the code it was not that complex in the end.
