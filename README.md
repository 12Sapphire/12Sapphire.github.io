<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>This is a Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 30px;
            background-color: #f9f9f9;
            color: #222;
        }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin-bottom: 25px;
        }
        h1 {
            font-size: 2.2em;
            margin-bottom: 15px;
            color: #2d4a70;
        }
        h3 {
            color: #23435c;
            margin-top: 30px;
        }
        a {
            color: #2a70b8;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        .about-me {
            background: #fff;
            padding: 20px 24px;
            border-radius: 10px;
            box-shadow: 0 3px 12px rgba(44,79,134,0.08);
            margin-bottom: 32px;
        }
        .thanks {
            font-size: 1.15em;
            font-weight: bold;
            color: #1e5a36;
        }
    </style>
</head>
<body>
    <h1>This is a Portfolio</h1>
    <img src="GithubWebsiteHeadline.png" alt="Github Website Headline">    
    <div class="about-me">
        <h3>About Me</h3>
        <p>
            I started when I was 9. I used a software called P5.js. I learned from Daniel Shiffman's YouTube channel called 
            <a href="https://www.youtube.com/@TheCodingTrain" target="_blank">The Coding Train</a>. 
            I made a 
            <a href="https://editor.p5js.org/F12/sketches/Db1CgRsBo" target="_blank">tree using fractals</a>, 
            <a href="https://editor.p5js.org/F12/sketches/-IKibwxcz" target="_blank">abstract art</a>, 
            <a href="https://editor.p5js.org/F12/sketches/vHkDAzvx-" target="_blank">drawing game</a>, + plus more.
        </p>
        <p>
            Fast forward 2 years, I used the "Elegoo Uno Super Starter Kit" that had been lying around. To start the Elegoo Uno R3 Super Starter Kit I watched the channel 
            <a href="https://www.youtube.com/@BV3D" target="_blank">BV3D</a>'s 
            <a href="https://www.youtube.com/playlist?list=PLWdhcCYoOsiJE1DS7OhPfwrHrGlUED6Az" target="_blank">Elegoo Uno Super Starter Kit Playlist</a> created by Bryan Vines. 
            I made a project with an IR receiver and IR remote control that prints sentences and words on Arduino IDE serial monitor. I also made one with a tilt ball switch that lights up a LED and turns on a buzzer if anyone touches the project.
        </p>
        <p>
            After a few months I decided to get a Raspberry Pi car from Freenove. After building and downloading everything, I had a lot of fun... for some days. But then the load button failed and only the wheels worked, and then the power button failed and it completely stopped working. I still don't know how to fix it yet.
        </p>
        <p>
            After a few weeks I went back to Arduino but this time I had to make a project that didn’t exist on BV3D. But BV3D did have 2 projects that I already had code for, and if I combined the code, I could use it in the new project. After wiring everything and uploading the code, my Temperature and Humidity Meter was done.
        </p>
        <p>
            Some days later, it was time to upgrade the Temperature and Humidity Meter with an ESP32 and Mosquitto. It was mostly easy, but accessing the temperature and humidity was confusing. So I asked an AI chat bot for help. And that’s how my Temperature and Humidity Meter was upgraded!
        </p>
    </div>
    <div class="thanks">
        Thanks!
    </div>
</body>
</html>
