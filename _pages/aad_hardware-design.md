---
layout: single
title: "Hardware Design"
permalink: /hardware-design/
author_profile: false
redirect_from:
  - /hardware-design
  - /hardware-design.html
---

The game has six buttons. Each button is connected to a GPIO port which is pulled up so that pressing the button is actually a low signal. Each of the buttons also has an LED which is connected to a solderboard which is connected to a 12V power supply. Each LED is individually connected to a 2N3904 transistor. The LEDs are also connected to individual GPIO pins. 

The mechanical structure of the game is a wooden box. There is an open front and open back for easy access to parts for assembling and wiring. The only thing that is visible to the player is the buttons on the top of the board. In the figure below, the frames of the boxes is shown.

After the frame was cut, we installed the 60 mm buttons into it. Each of the 60 mm buttons have 4 ports. 2 of the ports are for the button. 

The other 2 ports are for the LED within the button. The LEDs have a max voltage of 12 volts with a built-in resistor. We connected the LEDs to individual nmos transistors called 2N3904. The respective GPIO pins are connected through a 1k ohm resistor to the base of the transistor. The voltage supply is connected through the LED to the collector of the transistor. The emitter is connected through a 150 ohm resistor to ground. 

The button pins are connected directly to the GPIO pins. One of the wires is connected to the GPIO pin and the other wire is connected to ground. The GPIO pins have a built-in resistor and have a voltage of 3.3 V. The figure below shows the button circuit.

The values for the resistors we received from the previous project that used these buttons. After seeing their frame for their project, we decided to make our own. The buttons did give us some trouble, which is explained in more depth below in the software section.