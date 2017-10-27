# LEGO
HomeWork 4. Motion along the wall with ultrasound sensor. Innopolis University

## Project description
This project realizes motion LEGO robot along the wall with ultrasound sensor. As a stabilization of the system, PID controller is using. Source code written in LEGO Mindstorms.

## Work process description
![LEGO Mindstorm Robot](https://raw.githubusercontent.com/Stayer/lego/master/robot.jpg "LEGO Mindstorm Robot")

This is the robot that I assembled for assignment. There were no problems during the constructing process. I looked at the instructions and did everything in steps. For programming, I used the standard LEGO Mindstorms software, because it is the simplest.  You can program at Pothon, but this requires an additional SD card. I have some problems with installation Mono framework (requires for LEGO), because I'm on Mac OS.

![LEGO SDK](https://raw.githubusercontent.com/Stayer/lego/master/lego.png "LEGO SDK")
This is LEGO SDK for programming their robots. It's too hard to understand how this blocks works. I did PID controller with these parameters: Kp = 0.4, Ki = 0.0027 , Kd = 0.5. Target distance to the wall for ultrasonic sensor - 20 cm. Speed = 40.

I tried a lot of coefficients, the most difficult was Ki. Initially, the robot often turned and could not tune in for a long time, but a small coefficient solved this problem. Now he drives smoothly. I also tried to change distance to 10 cm, increase speed to 60 and 80, but it took bad results. This configuration is optimal.

When I'm trying to increase robot movement speed, system began to work poorly, robot started to turn in place. Most likely, the readings from the ultrasonic sensor are not taken off so often.

https://youtu.be/KokzeNlggvE
