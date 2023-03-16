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
### Developed By:POOJITHA.S
### Register Number: 212221240050
i) #To Read,display the image
```
import cv2
A=cv2.imread("photo.jpg",1)
cv2.imshow("212221240050",A)
cv2.waitKey(0)
 
```
ii) #To write the image
```
import cv2
A=cv2.imread("photo.jpg",1)
cv2.imwrite("photo.jpg",A)
cv2.imshow("212221240050",A)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```
import cv2
A= cv2.imread('photo.jpg',1)
print(A.shape)

```
iv) #To access rows and columns

```
import random
import cv2
A = cv2.imread('photo.jpg',1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240050',A)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
A= cv2.imread('photo.jpg',1)
tag = A[300:400,300:400]
A[90:190,90:190] = tag
cv2.imshow("212221240050",A)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image
![digital](https://user-images.githubusercontent.com/93427581/225594732-e15fe017-4ca4-4a9b-8608-a7d607fbe0a9.png)



### ii)Write the image
![digital1](https://user-images.githubusercontent.com/93427581/225594806-b8fb3d8b-5cc6-4463-9985-536c5bbcbc37.png)



### iii)Shape of the Image
![digital2](https://user-images.githubusercontent.com/93427581/225594870-5a3c1313-bca1-45c5-a9a4-170dd8952aaf.png)



### iv)Access rows and columns
![digital3](https://user-images.githubusercontent.com/93427581/225594936-9d1c9059-f800-4595-ab76-6c798872422f.png)



### v)Cut and paste portion of image
![digital4](https://user-images.githubusercontent.com/93427581/225595164-4de0bf40-e6f6-4b07-a603-cffced1b3f8a.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


