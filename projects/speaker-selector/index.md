---
title: SpeakerSelector 🔈📟
layout: page
permalink: /projects/speaker-selector/
---

![SpeakerSelectorFront](/assets/img/projects/speaker-selector/front.jpg)

## Description
A friend of mine, who's an audiophile, ran into a bit of a hassle—he owns three pairs of high-end speakers, each ideal for a different music genre. But every time he wants to switch genres, he has to manually swap speaker cables at his amplifier.
To solve this, I came up with an idea: an ESP8266-controlled relay switch that lets him easily switch between speaker pairs without touching a single cable.
The system has four independent stereo outputs, each controllable via dedicated buttons. Additionally, it hosts a small web interface on the local network for convenient remote control.
Source code can be found here: [EspSpeakerSelector](https://github.com/marcidelux/EspSpeakerSelector)

## Features:
- Remembers the selected speaker, SSID, and Wi-Fi password.
- Static webpage for setting up Wi-Fi credentials.
- Static webpage for controlling the relays.
- Built-in socket server for syncing the currently selected speaker across multiple clients.

## Demo
<div style="position: relative; width: 100%; padding-top: 56.25%; /* 16:9 aspect ratio */">
<iframe 
src="https://www.youtube.com/embed/Z5lwOLhOSss?si=PJgLGM0tm7P5--0D"
frameborder="0"
width="100%"
height="100%"
allowfullscreen="true"
style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
></iframe>
</div>

## Some more images
![SpeakerSelectorBack](/assets/img/projects/speaker-selector/back.jpg)
![SpeakerSelectorInside](/assets/img/projects/speaker-selector/inside.jpg)

