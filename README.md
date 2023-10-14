# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1 :
Import the necessary packages.

## Step 2 :
Create the Text using cv2.putText

### Step 3 :
Create the structuring element.

### Step 4 :
Use Opening operation.

### Step 5 :
Use Closing Operation.

## Program:
## DEVELOPED BY : JAYASRI DODDA
## REGISTER NO : 212222240028
## Import the necessary packages :
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
## Create the Text using cv2.putText :
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'JAYASRI D',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```
## Create the structuring element :
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
## Use Opening operation :
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
## Use Closing Operation :
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()
```
## Output :
## Display the input Image :
![Screenshot from 2023-10-14 15-49-25](https://github.com/jayasridodda/OPENING--CLOSING/assets/123259278/c05e10e9-a61d-450b-a931-b1e1524589cb)

## Display the result of Opening :
![Screenshot from 2023-10-14 15-49-32](https://github.com/jayasridodda/OPENING--CLOSING/assets/123259278/2129c40d-6976-4fed-ae0f-0a11bead4a26)

## Display the result of Closing :
![Screenshot from 2023-10-14 15-49-38](https://github.com/jayasridodda/OPENING--CLOSING/assets/123259278/675c8406-c8f3-4e3c-846b-f3165032cae0)

## Result :
Thus the Opening and Closing operation is used in the image using python and OpenCV.
