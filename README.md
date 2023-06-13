# Virtual_Mouse
An AI-based application which let us control the mouse cursor by moving finger in Air in front of Camera of device.

 ![final](https://user-images.githubusercontent.com/78357575/123516002-93aed580-d6b7-11eb-835b-ac7b284850d5.jpg)

<br>

## About the Project:
- The goal is to manage computers and others devices with gestures rather than pointing and clicking a mouse or touching a display directly.
- In this project we use a approach that uses a video device to control the mouse system (Mouse Task).

<br>

## Tech Stacks:
- OpenCV (for image processing and drawing)
- Mediapipe (for Hand Tracking)
- PyAutoGui (for controlling mouse movement and click)
- Numpy

<br>

## Prerequisites:
- Install python version 3.7 or more
- Import all modules required for the project using this command
```
pip install <module name>
```

<br>

## Hardware and Software Requirements:
1. Webcam:
   - cv2.VideoCapture(0) [For integrated Webcam]
   - cv2.VideoCapture(1) [For Externally Joined Webcam]
2. Required Libraries:
   - **OpenCV [Open Source Computer Vision Library]:** OpenCV library in python is a computer vision library that is widely used for image analysis, image processing, detection, recognition, etc.

   - **Mediapipe:**  It is a cross-platform library developed by Google that provides amazing ready-to-use ML solutions for computer vision tasks.

   - **AutoPy:** AutoPy is a simple, cross-platform GUI automation library for Python. It includes functions for controlling the keyboard and mouse, finding colors and bitmaps on-screen, and displaying alerts.

<br>

## Project Flow:
- Find Hand Landmarks.
- Get the tip of Index and middle fingers.
- Check which finger are up.
     Only Index finger up : Moving mouse
- Convert Coordinates.
- Smoothen Values.
- Move Mouse.
- Both Index and Middle fingers are up : Clicking mode.
- Find distance between fingers.
- Click mouse if distance are short. [distance to be specified]
- Show frame rate.
- Display the project i.e run virtual mouse. 


<br>

## Project Approach:
1. Image Resize :
	Map camera coordinates to screen coordinates.
 
2. Segmentation :
	Separate the hand area into RGB from a complex background.
 
3. Denoise:
	Need to delete noisy pixels from the image.
 
4. Compute Center:
	Draw a circle increasing the radius of the circle from the center coordinate until the circle meets the first black pixel.
	When the algorithm finds first black pixel the it returns to the current radius.
 
5. Controlling Mouse:
<br />-Mouse movement:
	When the algorithm detects only index finger up then mouse moves according to the speed of hand movement.
<br />-Left click:
	When there is index and middle finger both up and distance between them is significantly low then is left click![Project approach](https://github.com/bipulkarna97/Virtual_Mouse/assets/126940912/3817be58-ea1e-46b2-87cb-8ac5ccb2e24e)


<br>

## Features :
* Can Move Your Cursor corresponding to your Index finger movement
* Can track your hand in real-time

<br>

## Working :
* This project is a use case of Hand Tracking technology. 
* As soon as the user shows up his hand in the camera the application detects it & draws a bounding box around the hand.
* If User shows only Index Finger than he/she can Move Cursor.
* To Click, User's Index and Middle finger both should be Up simultaneously. 
 
<br>

## Hand Landmarks:
With the use of mediapipe python library we can detect face or hand landmarks based on our uses.

![Hand Landmarks](https://github.com/bipulkarna97/Virtual_Mouse/assets/126940912/3c541758-bdf3-4ba7-927b-d6c912920c42)

<br>

## Hand Tracking:
![Hand tracking run 1](https://github.com/bipulkarna97/Virtual_Mouse/assets/126940912/d33514f7-fd95-403c-93cf-03ddb8f7ad42)

<br>

## Packages Used:
![List of packages used](https://github.com/bipulkarna97/Virtual_Mouse/assets/126940912/475491a8-6b6f-44e7-95aa-315993fe5f44)

<br>

## Future Scope:
- Further, we plan to add more features such as enlarging and shrinking windows, closing window, etc. by using the palm and multiple fingers.
- We can also open the browser or any drives (C:/D:/E: etc) with help of hand gestures instead of moving of cursor.
- This system could also be useful in presentations and to reduce work space.

<br>

## Resources:
<a href="https://www.youtube.com/watch?v=8gPONnGIPgw" target="_blank">YouTube : Murtaza's Workshop - Robotics and AI</a> <br>
<a href="https://www.computervision.zone/courses/ai-virtual-mouse/" target="_blank">Computer Vision Zone Website : Murtaza's Workshop - Robotics and AI</a>

<br>
<br>
<h1 align="center">THANK YOU </h1>
