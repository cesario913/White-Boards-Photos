# White Boards Photos

*A way to digitalise your whiteboard !!!*

![assembly render](https://github.com/cesario913/White-Boards-Photos/assets/141003626/dd59fb81-cf28-4022-8600-96da3101a658)
*Beta V1.0*


> [!warning]
> This project is very much a WIP but there is an MVP (minimum viable product).
>
> The software side will be my next priority,
> for now i am using an example sketch for the esp32 cam (server) that allows to take and save photos over local wi-fi.

# Objectives

The goal of this project is to have an object that makes it easy for you to take pictures of what's on your whiteboard, be able to do this trough a physical button or over wi-fi, and have a SVG file stored in the cloud (ex. google drive) i would also like to have the possibility of choosing it as video input for discord, zoom etc.


Solutions to this problem already exist like the [logitech scribe](https://www.logitech.com/en-us/products/video-conferencing/room-solutions/scribe.960-001332.html) but i want to have my take on it and make it a lot more afordable.

> If you have ideas or toughts about this project feel free to tell me in the discussions tab.


# How to build it ?


You will need the following :

```
Hardware :
- ESP32 CAM + programming module
- OV2640 160º long cable 
- M5x30mm 2x
- M5x20mm 2x
- M5 nut 2x
- double sided foam tape
- USB type C breakout board (for BETA V1.0)
- external antenna (for BETA V1.0)
- M3x10mm 2x (for MVP)
- M5 wingnut (for MVP)
```
```
Tools :
HEX M5 & M3 allen keys
soldering iron (for BETA V1.0)
```

https://github.com/cesario913/White-Boards-Photos/assets/141003626/b958ab61-fa18-4025-aa7f-6af0de52a47b


## Instruccions for MVP cam holder : 

1. Print every STL in PLA 20 % fill

2. Install esp32 cam server example onto the esp32  

3. Apply the double sided tape to the backside of "fixation mur" and fix it to the wall in the correct orientation, close to the whiteboard and in the middle.

4. Thread the M5 x 30 mm bolt in "avant bras" and assemble it with "biceps"

5. Pass your micro-USB cable trough "fixation mur" first and then trough "biceps" & "avant bras" and bolt them together with 2x M5x20mm in oposed corners

6. Connect the camera module to the rest with an embeded nut in cam holder and an assembled knob, connect the cable

7. Ta - Da

You can now connect to the ip adress of the esp32 and take photos or start a live it will be probably quite slow the bottleneck is the antena wich will be external for upcoming versions.
In my testing i also had lots of noise and artifacts in the pictures this may be caused by the bad connection or power delivery. 


 

# known issues :

- there is too much play between "avant bras" & "biceps"
- the mounting holes to "fixation mur" are hard to access, they need to be on an angle


# Reference drawing for connecting parts :

The assembly has been created with modularity in mind here are the dimensions for you to create stuff 





# Licence :
[Attribution-NonCommercial 4.0 International
](https://creativecommons.org/licenses/by-nc/4.0/deed.en)


