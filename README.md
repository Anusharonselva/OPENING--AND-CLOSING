# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2:
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation
### Step5:
Use Closing Operation

 
## Program:
```
DEVELOPED BY: S.ANUSHARON
REG.NO: 212222240010
```
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'DataScience',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image2=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel)
plt.imshow(image2)
plt.axis("off")
```


## Output:

### Display the input Image
![Screenshot 2024-04-27 223141](https://github.com/Anusharonselva/OPENING--AND-CLOSING/assets/119405600/f8739dbe-36ae-4176-8cc4-f03cbb060111)


### Display the result of Opening
![Screenshot 2024-04-27 223154](https://github.com/Anusharonselva/OPENING--AND-CLOSING/assets/119405600/c913ad86-ca79-4735-92b0-d02827d09ad0)


### Display the result of Closing
![Screenshot 2024-04-27 223203](https://github.com/Anusharonselva/OPENING--AND-CLOSING/assets/119405600/24539b1c-2dc8-4f18-982e-33df235341c2)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
