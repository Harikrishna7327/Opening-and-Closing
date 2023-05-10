# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:

## Step 1:
Import the necessary packages.

## Step 2:
Create the Text using cv2.putText

## Step 3:
Create the structuring element.

## Step 4:
Use Opening operation.

## Step 5:
Use Closing Operatio
 
## Program:

```
/*
Developed by   : M.Hari krishna
Register Number: 212221230059
*/
# Import the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText

img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img, 'Hari krishna ',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()

# Create the structuring element 

kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))

# Use Opening operation

image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()

# Use Closing Operation

image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()




```
## Output:

### Display the input Image

![image](https://github.com/Harikrishna7327/Opening-and-Closing/assets/94882905/6283ab38-6b74-4ade-9b3c-360cc72caba9)

### Display the result of Opening

![image](https://github.com/Harikrishna7327/Opening-and-Closing/assets/94882905/7ae973d9-c6ed-4b75-9685-b223e0834234)

### Display the result of Closing

![image](https://github.com/Harikrishna7327/Opening-and-Closing/assets/94882905/a75f16ae-5004-4219-ae8b-a00903e9fcfd)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
