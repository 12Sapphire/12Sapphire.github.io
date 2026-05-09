###### 2026
# Landslide Detection System
In this project, I'll be making a simple landslide detection device for a tech showcase.

First, I wanted a landslide that activated with a spray bottle that to stimulate rain since heavy rain is the most common cause of landslides.  But soon I found out water is too messy for a showcase and none of the tests I did worked. I ended up making a manually controlled slop that mimiced how a real landslide would happen.

Then I started working on the device.I wanted it to alert a landslide would happen wirelessly by Mosquitto. The hardware I used was an ESP32 board and IMU sensor. For the software, I used the Arduino IDE and a new software that I'm unfamiliar with which is Google's Antigravity. 

I started by prompting Antigravity to build a simple landslide detection device that detects downward movement alerts a landslide might happen through Mosquitto with an IMU sensor and an ESP32 board.After running the code,I found out that the type of IMU Antigravity assumed I had (I also assumed I had that one) was wrong. After changing the IMU type, I couldn't find the new library I needed. So I told Antigravity to change the library. After changing the library, the code wouldn't compile. Antigravity couldn't fix it. I gave the code to gemini and it told me that the new library had "arduino" written in it instead of "Arduino" and I fixed it manually. Later I found out I hadn't given Antigravity access to that library and thats why it was taking so long and couldn't fix the problem. Tere were a few mosre small errors that were fixed. When the code was uploaded, nothing showed up. On the serial plotter it showed there was 
