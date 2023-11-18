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
- u.fl external antenna (for BETA V1.0)
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

## Here are some videos to help you :

- [esp32 cam presentation and how to install server example ](https://www.youtube.com/watch?v=visj0KE5VtY&ab_channel=DroneBotWorkshop)
if you use the programming module for esp32 cam you don't need the FTDI presented in the video just a micro usb cable directly connected to the computer

- [more in depths look at the camera OV2640 itself and how to change between cameras](https://www.youtube.com/watch?v=jbQ9Bp3wE_w&ab_channel=ThatProject) 

# Status of the repo :

There is one working version the MVP.
For now the physical design will not change except for the camera module that needs more work and the future addition of a button. The focus will be more on the coding.  


## known issues :

- there is too much play between "avant bras" & "biceps"
- the mounting holes to "fixation mur" are hard to access, they need to be on an angle

## What comes next/ where to help :

I haven't decided on a couple of stuff, how the interface would be or behave for example if you connect your computer to it trough an app maybe bluetooth etc, but I am open to suggestions.
The progresss will be in "modules" that can later be sawn together.

### Programming :

- a python program that can detect where is the white board and apply a perspective transform to the picture and other image manipulation
- a way to send a request to take picture and download it directly to the computer in a specific folder

### 3d modeling :

- A camera module that holds the esp32 and camera for easy prototyping (with pins in the open)

# Reference drawing for connecting parts :

The assembly has been created with modularity in mind here are the dimensions for you to create stuff 

(will come)



# Licence :
[Attribution-NonCommercial 4.0 International
](https://creativecommons.org/licenses/by-nc/4.0/deed.en)


