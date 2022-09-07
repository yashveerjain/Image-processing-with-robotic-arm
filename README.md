# Image-processing-with-robotic-arm
## About:
* This Robot was built for the segragation of metallic round object, which can be used in industries or for garbage segregation if fix sized and shape object need to be segregated.

## Technical Details: The project was divided in two parts:
1. Hardware: Hardware needed was a -> 2MP logitech Webcam,2 Sparkfun EasyDriver, Raspberry pi, Arduino.
2. Software: Contains 2 parts
    - The code is written in python, dependent on opencv, numpy and imported the library pyfirmata for communicating with the arduino and then run the example of standard firmata library in arduino.
    - Computer Vision for detecting the objects in the image frame and it location, method used background subtraction, and connective labelling to separate each object and calculate its centroid in the pixel coordinate, and then converted to Cartesian coordinate (x-y plane in cm) feeding it to 2ndt part of the software.
    - Running the hardware, according to specific x-y coordinate converting to the stepper rotation and controlling the stepper motor

## Device image
![](images/industrial-robot.png)

## Device working videos
* [demo video](https://drive.google.com/file/d/1eLh3OXNollj0qVDoGT9Q1KkzQ-V80hNA/view?usp=sharing) for single object localization and tracing.

* [demo video](https://drive.google.com/file/d/1hKvEndr-Cx-MMgwWZ3WBfSbs_qFxjQ0z/view?usp=sharing) for multi object localization and tracing.
