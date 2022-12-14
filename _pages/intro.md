---
permalink: /
layout: single
title: "Introduction"
author_profile: false
redirect_from:
  - /intro/
---

Link to our [demo](https://www.youtube.com/watch?v=SYxIqJ6wqH0&list=PLDqMkB5cbBA6AwYC_DElkDStUdOsTuIL7&index=8). Note that in the Appendix section we state that we approve of this video and site being on the course site.

### Syyynth Hero: where synth legends are made.
We created a game that is a cross between Piano Tiles and Guitar Hero, made to teach you how to play the synth with a variety of songs to choose from. We started this project with the intent of making a game that could teach you how to play an instrument using songs and a button system. Our project was inspired by rhythm games like Piano Tiles and Guitar Hero, and our interface looks like a simplified version of these games, with tiles (called NoteBars) that progress down the screen. When you press one of the buttons, it plays a corresponding note. The goal is to correctly press the notes of each song at the right time until the song ends. Correctly pressing a note increases your score, and the goal is to get the highest score possible. A player knows when the button needs to be pressed because the tile overlaps with the scoreline on the VGA screen, and the button lights up as well. We hope you enjoy our creation and hopefully get to try to play the game at some point! 

<p align = "center">
<img src="/images/a_images/intro/stock.png" alt="image" style="width:70%">
</p>
<p align = "center">
Image of the game's main menu
</p>
<br>
<p align = "center">
<img src="/images/a_images/intro/notebars.png" alt="image" style="width:70%">
</p>
<p align = "center">
Image of gameplay which contains 3 NoteBars on screen
</p>

&nbsp;
### Brief Overview of Development Process
We started the project by designing the GUI (Graphical User Interface) and displaying that design to the VGA monitor, since that is the aspect of the project that can be easily changed and for which we could make visible progress. This started as drawing the main game screen, to adding randomly floating notes that would come down the screen and wait to be clicked. We then designed the mechanical aspect of the game which had the buttons and laser-cut wooden frame for the arcade-like system we had. Once this was built, we tested each of the buttons by connecting them to the RP2040 and displaying a distinct output to the VGA screen. At this point, we had a working prototype similar to Piano Tiles but without any music. We then used direct-digital synthesis (like in the crickets lab) to simulate the sound of a synth and created a standard data-form for which we could add multiple songs the user could choose to play. The finishing touch was making the LEDs attached to the buttons light up when the tile corresponding to the button was on the black line, indicating the user should press the button. Once we finished this, we had a fully functional Syynth Hero game!