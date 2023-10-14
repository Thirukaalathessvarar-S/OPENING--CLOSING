# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step1:
### Step1: Import the necessary packages.
### Step2: Read the image.
### Step3: Create the structuring element or kernal element.
### Step4: Use Opening operation.
### Step5: Use Closing Operation.

## Program:

```
import cv2
import numpy as np
img=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img,'Eswar_212222230161',(5,60),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("Original Image",img)

kernal=np.ones((5,5),np.uint8)
imgO=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernal)
cv2.imshow("Opening Operation",imgO)
imgC=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernal)
cv2.imshow("Closing Operation",imgC)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![exp11_1](https://github.com/Thirukaalathessvarar-S/OPENING--CLOSING/assets/121166390/3ab3a51d-5f83-40d3-93ee-8ad9c0d60b5f)


### Display the result of Opening
![exp11_2](https://github.com/Thirukaalathessvarar-S/OPENING--CLOSING/assets/121166390/d398cea2-bde5-4b32-9f3d-d9246be4a0f2)

### Display the result of Closing
![exp11_3](https://github.com/Thirukaalathessvarar-S/OPENING--CLOSING/assets/121166390/a00a6b23-b73a-4527-9a93-885d767f4755)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
