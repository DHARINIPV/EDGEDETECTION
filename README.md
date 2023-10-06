# EDGEDETECTION

## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

### Step2:
For performing edge detection on a image.

### Sobel
sobelx=cv2.Sobel(gray,cv2.CV_64F,1,0,5)

sobely=cv2.Sobel(gray,cv2.CV_64F,0,1,5)

sobelxy=cv2.Sobel(gray,cv2.CV_64F,1,1,5)

### Laplacian
lap=cv2.Laplacian(gray,cv2.CV_64F)

### Canny
canny=cv2.Canny(gray,120,150)

### Step3:
Display all the images with their respective edge detected images.

## Program:

Developed by: Dharini PV
Register no : 212222240024

# Import the packages
```python
import cv2
import matplotlib.pyplot as plt
```
# Load the image, Convert to grayscale and remove noise
```python
img=cv2.imread("thor.jpeg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
```
# SOBEL EDGE DETECTOR
SOBEL X AXIS :
```python
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.figure(figsize=(7,7))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelx)
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
SOBEL Y AXIS :
```python
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.figure(figsize=(7,7))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobely)
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
SOBEL XY AXIS :
```python
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize=(7,7))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelxy)
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
# LAPLACIAN EDGE DETECTOR
```python
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.figure(figsize=(7,7))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(lap)
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
# CANNY EDGE DETECTOR
```python
canny=cv2.Canny(gray,120,150)
plt.figure(figsize=(7,7))
plt.subplot(1,2,1)
plt.imshow(gray)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(canny)
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
### SOBEL EDGE DETECTOR

SOBEL X AXIS :

![Screenshot from 2023-10-06 23-59-56](https://github.com/DHARINIPV/EDGEDETECTION/assets/119400845/bad11f3d-9f5b-42fb-95b1-52a0f07ec11f)

SOBEL Y AXIS :

![Screenshot from 2023-10-07 00-00-36](https://github.com/DHARINIPV/EDGEDETECTION/assets/119400845/a869f30d-3d59-4fa9-a4cf-0e9f35d85755)

SOBEL XY AXIS :

![Screenshot from 2023-10-07 00-01-06](https://github.com/DHARINIPV/EDGEDETECTION/assets/119400845/4b7bc780-ebbf-42fd-a310-67635a25016c)

### LAPLACIAN EDGE DETECTOR
![Screenshot from 2023-10-07 00-01-43](https://github.com/DHARINIPV/EDGEDETECTION/assets/119400845/72bf21d4-7fd1-48ed-b8b5-d081f624b9d1)

### CANNY EDGE DETECTOR
![Screenshot from 2023-10-07 00-02-25](https://github.com/DHARINIPV/EDGEDETECTION/assets/119400845/92be3512-050d-4439-ac7f-301ed0fc44c5)

## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
