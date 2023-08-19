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
```
Developed By : D.vishnu vardhan reddy
Register Number : 212221230023
```
#### To Read,display the image
```
import cv2
color_img=cv2.imread('ram.jpg',1)
cv2.imshow('212221230023 VISHNU',color_img)
cv2.waitKey(0)  


```
### To write the image
```
import cv2
color_img=cv2.imread('ram.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221230023 VISHNU',color_img)
cv2.waitKey(0) 


```
### Find the shape of the Image
```

import cv2
import random
color_img=cv2.imread('ram.jpg',1)
print(color_img.shape)

```
### To access rows and columns

```
import cv2
import random
color_img=cv2.imread('ram.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230023 VISHNU',color_img)
cv2.waitKey(0)



```
### To cut and paste portion of image
```
import cv2
color_image=cv2.imread('ram.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212221230023 VISHNU',color_image)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image
![image](https://github.com/vishnudorigundla/READ-AND-WRITE-IMAGE/assets/94175324/375dc993-47b4-4307-9dae-24b47a33240a)



### ii)Write the image

![image](https://github.com/vishnudorigundla/READ-AND-WRITE-IMAGE/assets/94175324/71b529da-63cb-4f77-9189-5b85fdf47a68)


### iii)Shape of the Image

![image](https://github.com/vishnudorigundla/READ-AND-WRITE-IMAGE/assets/94175324/9423e9a4-22e3-4841-9995-7ef2c83b6ae8)


### iv)Access rows and columns
![image](https://github.com/vishnudorigundla/READ-AND-WRITE-IMAGE/assets/94175324/e0f16711-0550-4dac-96f5-ff3b6b3cdba3)

### v)Cut and paste portion of image

![image](https://github.com/vishnudorigundla/READ-AND-WRITE-IMAGE/assets/94175324/54c0c58f-8a88-4e28-aa87-e57c463f4bd7)

## Result:
Thus the images are read, displayed, and written successfully using the python program.

