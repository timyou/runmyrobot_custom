# runmyrobot
Robot controller and video scripts


Robot Controller

Installation:

(1) Install motor HAT
https://learn.adafruit.com/adafruit-dc-and-stepper-motor-hat-for-raspberry-pi/installing-software

(2) pip install socketIO-client


How to run:

Go to new robot page to create a robot. If you already have one, got to manage robots. There you'll find your Robot ID and Camera ID.

<h2> Programs to run on the Raspberry Pi: </h2>

These two scripts need to be running in the background to bring your robot to life: controller.py, send_video.py. Here are instructions about how to start them.

Starting the Robot Controller for the Robot

python controller.py YOUR_ROBOT_ID

For example:

```python controller.py 789123```




Starting the Video Streamer for the Robot


```python send_video.py YOUR_CAMERA_ID YOUR_VIDEO_DEVICE_NUMBER```

For example:

```python send_video.py 12345 0```

The second parameter 0 is assuming you have one camera plugged into your Pi and you are using it, which is usually the case.




How to enhance your bot with an Android phone:

Android phone will provides streaming Audio (robot to user), text to speech, and orientation information to prevent flipping. You can download the app-debug.apk file and run it as an app on your phone. Note that the phone needs to be oriented face up with the right side of the phone facing the forward moving direction of the robot.


