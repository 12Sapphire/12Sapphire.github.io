###### 2026
# Landslide Detection System
In this project, I'll be making a simple landslide detection device for a tech showcase.
## Why I Chose This Project
In the area we live in, landslides are a major problem and current tech used for detection can be expensive, hard to deploy, and older versions can lack cloud connection. I thought we could make a better device that is cheap, easy to deploy, and connected to the cloud. (Thic project is ONLY a project and I'm not planning to scale it up)

## How I built it

First, I wanted a landslide that activated with a spray bottle to simulate rain, since heavy rain is the most common cause of landslides. But soon, I found out water is too messy for a showcase, and none of the tests I did worked. I ended up making a manually controlled slope that mimicked how a real landslide would occur.

Then, I started working on the device. I wanted it send alerts wirelessly through Mosquitto. The hardware I used was an ESP32 board and an IMU sensor. For the software, I used the Arduino IDE and Google's Antigravity.

I started by prompting Antigravity to build a simple landslide detection device that detects downward movement and alerts that a landslide might happen through Mosquitto using an IMU sensor and an ESP32 board.

After running the code, I found out that the type of IMU Antigravity assumed I had (which I also assumed I had) was wrong. After changing the IMU type, I couldn't find the new library I needed, so I told Antigravity to change the library. After changing the library, the code wouldn't compile. Antigravity couldn't fix it. I gave the code to Gemini, and it told me that the new library had "arduino" written in it instead of "Arduino," and I fixed it manually. Later, I found out I hadn't given Antigravity access to that library, and that's why it was taking so long and couldn't fix the problem. There were a few more small errors that were fixed.

When the code was uploaded, the Serial Monitor gave weird readings, and nothing showed up on the terminal. I decided to first get the readings correct on the Serial Monitor. After many errors and weird messages, the readings were finally correct. Although the data (which was written weirdly) was coming in way too fast, and the sensitivity was too low. I told Antigravity to change it so that it only showed major changes in movement and increased the sensitivity. It became worse; it made it so that it gave an alert after every certain amount of time, even when I didn't move the IMU sensor. (Maybe it is my fault and how I use Antigravity.) Luckily, I copied the original code and pasted it back. Later, I changed it so it only gave data readings every 3 seconds and changed the sensitivity manually.

Although the data was okay on the Serial Monitor, it couldn't connect to the MQTT broker. It didn't work for a few days, but in the end, the server was changed to HiveMQ, and some other adjustments were made. Then, it finally sent data to the MQTT server.

After that, I made a dashboard to present the data cleanly.

A few adjustments later, the project was finally ready to be showcased.


