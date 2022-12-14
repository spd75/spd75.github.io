---
layout: single
title: "Appendix"
permalink: /appendix/
author_profile: false
---


### Appendix A - Approval to Use Report
The group approves this report for inclusion on the course website.
The group aprroves the video for inclusion on the course youtube channel.


### Appendix B - Code
The code for the project can be found at the following GitHub link. Please note that all of the code found on this GitHub repository needs to be located within Professor Adams' lab directory to run successfully.

[Local Project Directory](https://github.com/spd75/ece4760-final)


### Appendix C - Schematics
All schematics can be found under the respective sections. However, here they are again.

<br>
<p align = "center">
<img src="/images/a_images/hardware/buttons.png" alt="image" style="width:74%">
</p>
<p align = "center">
Button schematic
</p>
<br>

<br>
<p align = "center">
<img src="/images/a_images/hardware/transistors.png" alt="image" style="width:64%">
</p>
<p align = "center">
Transistor circuit with base connecting to GPIO pins
</p>
<br>

<br>
<p align = "center">
<img src="/images/a_images/hardware/all.png" alt="image" style="width:64%">
</p>
<p align = "center">
Schematic including all buttons and LEDS - note that buttons and LEDs are together in real life, but we separated them here to simplify visuals
</p>
<br>

<br>
<p align = "center">
<img src="/images/a_images/hardware/audio.png" alt="image" style="width:60%">
</p>
<p align = "center">
Schematic for sound production part of our project.
</p>
<br>

<br>
<p align = "center">
<img src="/images/a_images/hardware/vga.png" alt="image" style="width:60%">
</p>
<p align = "center">
Schematic for VGA connections.
</p>
<br>


### Appendix D - Work Breakdown
The group consisted of Emmanuel and Sergio. 

Sergio's Tasks:
* Primary software writer and designer
* Assistance with hardware wiring

Emmanuel's Tasks:
* Assistance with software
* Hardware wiring
* Laser-cut board


### Appendix E - Cost List
Here is the Price of our Project:
* Plywood (Cornell Store) - $16
* Large Arcade Yellow Button x2 (Adafruit) - $5.95 * 2
* Large Arcade Blue Button x2 (Adafruit) - $5.95 * 2
* Large Arcade Red and Green Button (Adafruit) - $5.95 * 2
* MCP 4802/4812/4822 (DigiKey) - $2.50
* Power Supply (ECE Lab) - $0
* VGA Monitor (ECE Lab) - $0
* Wires, boards (ECE Lab) - $0

Total Spent on Project: $54.20


### Appendix F - References
Insperation for our laser cut and button design came from the Whack-a-Button project from last year. We also used the same buttons they used. Their website can be found here:

[Whack-a-Button](https://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2021/hl693_jw829_ap845/hl693_jw829_ap845/index.html)

Insperation for direct digital synthesis code can be found here:

[DDS Example in Code](https://github.com/vha3/Hunter-Adams-RP2040-Demos/blob/master/Lab_1/Audio_Beep_Synthesis/multitest.c)

We used the Pico SDK. This can be found here:

[RP2040 Pico SDK](https://github.com/raspberrypi/pico-sdk)

We used VGA driver for VGA communication between the RP2040 and the VGA monitor. More information about that can be found here:

[VGA Driver](https://vanhunteradams.com/Pico/VGA/VGA.html)

We used the RP2040 datasheet. This can be found here:

[RP2040 Datasheet](https://datasheets.raspberrypi.com/pico/pico-datasheet.pdf)

We used DAC datasheet. This can be found here:

[MCP4802/4812/4822 Datasheet](https://vanhunteradams.com/Pico/Cricket/DAC.pdf)

We used the C SDK guide. This can be found here:

[RP2040 C SDK Guide](https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-c-sdk.pdf)
