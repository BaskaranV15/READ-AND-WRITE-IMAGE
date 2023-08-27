![dig1](https://github.com/BaskaranV15/READ-AND-WRITE-IMAGE/assets/118703522/dc60feb8-1405-4644-b2fe-cf1830017e86)# READ AND WRITE AN IMAGE
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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
image=cv2.imread("image1.png",1)
cv2.imshow('212222230020_baskaran',image)
cv2.waitKey(0) 
```
ii) #To write the image
```
import cv2
image=cv2.imread("image1.png",1)
w=cv2.imwrite('i.png',image)
cv2.imshow('212222230020_baskaranv',image)
cv2.waitKey(0) 
```
iii) #Find the shape of the Image
```python3
import cv2
import random
image=cv2.imread("image1.png",1)
print(image.shape)
```
iv) #To access rows and columns

```python3
import cv2
import random
image=cv2.imread("image1.png",1)

for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230020_baskaran',image)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```python3
import cv2

image=cv2.imread("image1.png",1)
image.shape
tag=image[350:550,200:350]
image[70:270,200:350]=tag
cv2.imshow('212222230020_baskaran',image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
![dig1](https://github.com/BaskaranV15/READ-AND-WRITE-IMAGE/assets/118703522/ede8c40b-2e0a-4f5d-8503-24c8b32db96b)

### ii)Write the image
![dig1](https://github.com/BaskaranV15/READ-AND-WRITE-IMAGE/assets/118703522/e3928f5c-7736-4005-8ba2-3ed7ca9b69ad)
### iii)Find the shape of the Image
![Screenshot from 2023-08-27 14-04-50](https://github.com/BaskaranV15/READ-AND-WRITE-IMAGE/assets/118703522/92acc9a9-30fc-408d-87de-056e9d72d09f)

### iv)Access rows and columns

file:///home/sec/Pictures/Screenshots/Screenshot%20from%202023-08-24%2021-40-56.png

### v)Cut and paste portion of image
![Screenshot from 2023-08-24 22-30-13](https://github.com/BaskaranV15/READ-AND-WRITE-IMAGE/assets/118703522/8e72cd20-76f4-44f7-90b1-75c5eedc7b0a)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
