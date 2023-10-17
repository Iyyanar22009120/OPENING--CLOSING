# OPENING--CLOSING
## Aim:
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:

### Step1:
Import the necessary packages.
<br>

### Step2:
Create the Text using cv2.putText.
<br>

### Step3:
Create the structuring element.
<br>

### Step4:
Use Opening operation
<br>

### Step5:
Use Closing Operation
<br>

 
## Program:

DEVELOPED BY: IYYANAR S

REGISTER NUMBER: 212222240036


## Import the necessary packages
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
```

## Create the Text using cv2.putText
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
cv2.putText(img1,'IYYANAR S',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')
plt.title('Input Text'), plt.xticks([]), plt.yticks([])
plt.show()
```

## Create the structuring element
```
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```

## Use Opening operation
```
image1=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernel1)
plt.imshow(image1,cmap='gray')
plt.title('OPENING'), plt.xticks([]), plt.yticks([])
plt.show()
```

## Use Closing Operation
```
image1=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel1)
plt.imshow(image1,cmap='gray')
plt.title('CLOSING'), plt.xticks([]), plt.yticks([])
plt.show()
```

## Output:

## Display the input Image
![10](https://github.com/Iyyanar22009120/OPENING--CLOSING/assets/118680259/a8ea84ee-3e25-4a85-a95c-a432162cba69)

<br>
<br>

## Display the result of Opening
![20](https://github.com/Iyyanar22009120/OPENING--CLOSING/assets/118680259/b3eab975-d141-4bd0-a384-25c88b1cabf2)

<br>
<br>

## Display the result of Closing
![30](https://github.com/Iyyanar22009120/OPENING--CLOSING/assets/118680259/c8f81236-21b5-4397-8aa6-df77e90094b2)

<br>
<br>


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
