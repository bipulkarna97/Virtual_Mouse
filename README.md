# Virtual_Mouse
An AI-based application which let us control the mouse cursor by moving finger in Air in front of Camera of device.

 ![final](https://user-images.githubusercontent.com/78357575/123516002-93aed580-d6b7-11eb-835b-ac7b284850d5.jpg)

### Tech Stacks:💻
- OpenCV (for image processing and drawing)
- Mediapipe (for Hand Tracking)
- PyAutoGui (for controlling mouse movement and click)
- Numpy

## Prerequisites:
- Install python version 3.7 or more
- Import all modules required for the project using this command
```
pip install <module name>
```

## Features :
* Can Move Your Cursor corresponding to your Index finger movement
* Can track your hand in real-time

### Working :
* This project is a use case of Hand Tracking technology. 
* As soon as the user shows up his hand in the camera the application detects it & draws a bounding box around the hand.
* If User shows only Index Finger than he/she can Move Cursor.
* To Click, User's Index and Middle finger both should be Up simultaneously. 
 
 



