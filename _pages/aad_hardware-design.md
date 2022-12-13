---
layout: single
title: "Hardware Design"
permalink: /hardware-design/
author_profile: false
redirect_from:
  - /hardware-design
  - /hardware-design.html
---

### Buttons and LEDS
The mechanical structure of the game is a wooden box. There is an open front and open back for easy access to parts for assembling and wiring. The only thing that is visible to the player is the buttons on the top of the board. In the figure below, the frames of the boxes is shown.

<br>
<p align = "center">
<img src="/images/a_images/hardware/box.png" alt="image" style="width:90%">
</p>
<p align = "center">
Schematic for VGA connections.
</p>
<br>

After the frame was cut, we installed the 60 mm buttons into it. The game has six buttons connected to this wooden box. Each of the 60 mm buttons have four ports. Two of these ports are used for the button's output signal that is then input into the RP2040. One wire is connected to a GPIO pin and the other wire is connected to ground. The GPIO pins have a built-in resistor and have a voltage of 3.3 V. In the software, we pull up these GPIO pins so that a LOW signal indicates that the button has been pressed. The figure below shows the button circuit.

<br>
<p align = "center">
<img src="/images/a_images/hardware/buttons.png" alt="image" style="width:74%">
</p>
<p align = "center">
Button schematic
</p>
<br>

The other 2 ports on the button control the LED which is connected to a solderboard which is connected to a 12V power supply. Each LED is individually connected to a 2N3904 transistor. The base of these transistors are then connected to GPIO pins through a 1k ohm resistor. The voltage supply is connected through the LED to the collector of the transistor. The emitter is connected through a 150 ohm resistor to ground.

<br>
<p align = "center">
<img src="/images/a_images/hardware/transistors.png" alt="image" style="width:64%">
</p>
<p align = "center">
Transistor circuit with base connecting to GPIO pins
</p>
<br>

The values for the resistors we received from the previous projects are the ones that used these buttons. After seeing their frame for their project, we decided to make our own. The buttons did give us some trouble, which is explained in more depth below in the software section.

<br>
<p align = "center">
<img src="/images/a_images/hardware/all.png" alt="image" style="width:64%">
</p>
<p align = "center">
Schematic including all buttons and LEDS - note that buttons and LEDs are together in real life, but we separated them to simplify visuals
</p>
<br>

### Audio
We also utilized the RP2040's SPI features to output audio that was generated via direct digital synthesis. A MCP4802/4812/4822 DAC was used to take in this SPI signal from the RP2040 and convert it from a digital signal to an analog signal. Both of the DAC's input channels were used as we did generate some audio concurrently whenever a user pressed more than one button at once. The output of the DAC was then connected to a 3.5 mm audio socket (aux) which allowed for a speaker to be plugged-in to synthesize our audio. A diagram of this circuit is shown below.

<br>
<p align = "center">
<img src="/images/a_images/hardware/audio.png" alt="image" style="width:60%">
</p>
<p align = "center">
Schematic for sound production part of our project.
</p>
<br>


### Visuals
For the visuals, we used a VGA screen and a VGA library that used DMA to send data to the VGA monitor without using up an CPU cycles. This library abstracted everything for us nicely so that we only had to use high-level functions such as drawRect() and fillRect(). As for the hardware aspect, we wired HSync and VSync directly from RP2040 ports, as well as the R, G, and B wires, which were connected to the VGA cable using 330 ohm resistors. A schematic of this can be seen below.

<br>
<p align = "center">
<img src="/images/a_images/hardware/vga.png" alt="image" style="width:60%">
</p>
<p align = "center">
Schematic for VGA connections.
</p>
<br>

