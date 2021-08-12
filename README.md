# Virtual-Paint
![5_6093884485021991981](https://user-images.githubusercontent.com/86593289/129163048-44bf3f84-3500-4a57-ad6c-0ff672d78d3d.png)

I have created this Virtual Paint Program, in this you can paint(draw) on your screen using hand gestures, created in Python-3.

**Gestures :-**
* Index Finger - for drawing
* Index+Middle Finger - for changing position and objects

# Code
Firstly I have created a Module "HandTrackingModule.py", this file contains the code which detects our hand, in this file I have created functions for specific tasks in a class "handDetector()". 

**Short description of functions are -**

* findHands() - This function detect hands and show landmarks of your hand and it return image in RGB.
* findPosition() - This function finds the position of particular landmark of your hand and it returns a list containing *id_of_that_landmark, x_position_of_that_landmark, y_position_of_that_landmark*.
* fingersUp() - This function check wheather your particular finger is up or not and it return a list containing values 0 (if finger is down) ans 1 (if finger is up). i.e. \[0,0,0,0,0] if all the 5 fingers are down and \[1,1,1,1,1] if all the fingers are up.

Then another file is "VirtualPaint.py", this file uses that HandTrackingModule and contains the code which draw on the screen and provide various features (3 Colors + Eraser).

This project is created in Python-3 language using OpenCV and Mediapipe libraries.
