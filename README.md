# Lane Detection
## Overview
Different approaches to find lane-lines on roads. The code is mostly based on Udacity's [self driving car program](https://eu.udacity.com/course/self-driving-car-engineer-nanodegree--nd013).

## Dependencies

Use Python 3.6 and install virtualenv (virtual environment)
```
sudo apt-get install python3-pip python3-dev python-virtualenv
``` 
Go to your home directory and create a virtualenv environment
```
virtualenv --system-site-packages lane_detection
```
Activate the virtualenv environment (use ```deactivate``` to exit)
```
source ~/lane_detection/bin/activate
```
Clone the Repo, cd into the folder and install all other dependencies in the requirements.txt file:
```
pip3 install -r requirements.txt
```

## Usage

### ProjectI: Simple Lane Detection

### ProjectII: Advanced Lane Detection

Use an advanced computer vision pipeline to extract features and determine lane-lines even in curved environments. Code works roughly as follows:

(1) Compute a camera calibration matrix and distortion coefficients given a set of chessboard images.

(2) Apply a distortion correction to raw images.

(3) Use filtering like edge detection, etc., to create a binary image.

(4) Apply a perspective transform ("birds-eye view").

(5) Apply a histogram to get lane pixels.

(6) Determine the curvature radius vehicle offset

(7) Warp all detected lane boundaries back to the original image.

(8) Output visual display 

Run the code with ```python3 P2.py ```

### ProjectIII: Advanced Lane Detection with Object Detection

### ProjectIV: SegNet Lane Detection



## Credits

The credits for this code go to [Udacity](https://github.com/udacity) and [georgesung](https://github.com/georgesung/advanced_lane_detection). I  mainly refactored the code and did some bugfixes.
