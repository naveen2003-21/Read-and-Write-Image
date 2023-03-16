# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: A Naveen Kumar
### Register Number: 212221240032
i) #To Read,display the image
```
import cv2
import matplotlib.pyplot as plt
from google.colab.patches import cv2_imshow
import random
image=cv2.imread("bike.jpg",-1)
cv2_imshow(image)

```
ii) #To write the image
```
image= cv2.imread('bike.jpg',-1)
cv2.imwrite('bike.jpg',image)


```
iii) #Find the shape of the Image
```
print(image.shape)

```
iv) #To access rows and columns

```
image = cv2.imread('bike.jpg',-1)
for i in range(150):
    for j in range(image.shape[1]):
        image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(image)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```
image= cv2.imread('bike.jpg',-1)
new = image[200:450,200:450]
image[150:400,150:400] = new
cv2_imshow(image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>
<br>

### ii)Write the image

<br>
<br>

### iii)Shape of the Image

<br>
<br>

### iv)Access rows and columns
<br>
<br>

### v)Cut and paste portion of image
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


