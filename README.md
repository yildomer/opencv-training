# freecodecamp OpenCV Tutorial

## Installation

python --version

pip install opencv-contrib-python
            opencv-python (main module)

NumPy: scientific computing library

pip install caer (speed up workflow) (?)

## Reading Images and Videos

import cv2 as cv
variable = cv.imread('path')
cv.imshow('nameofwindow', variable)
cv.waitKey(0) 
- (keyboard binding) 

### Reading Videos

capture = cv.VideoCapture('path'/0/1/...)
- 0: webcam 0
- 1: webcam 1 
- ...

~~~
while True:
    isTrue, frame = capture.read()
    cv.imshow('nameWindow', frame)

    if cv.waitKey(20) (?) & 0xFF == ord('d') (?):
        break

capture.release()
cv.destroyAllWindows()
~~~

Error message -215:Assertion failed

Could not find the media file, video run out of frames, it is done.

13:00