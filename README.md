# image-processing
1.	Develop a program to display gray scale image using read and write operation.

cv2.imread() -  loads an image from the specified file.
cv2.imshow() - to display an image in a window.
cv2.cvtColor() - used to convert an image from one color space to another.
cv2.imwrite() - used to save an image to any storage device.
         import cv2 
         image=cv2.imread("dog.jpg")
         cv2.imshow('Original Image',image)
         cv2.waitKey(0)
         gray_img = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
         cv2.imwrite('gray scale',gray_img)
         cv2.waitKey(0)
         cv2.destroyAllWindows()

Output:
![image](https://user-images.githubusercontent.com/72515142/104429740-f7cb5a80-55ab-11eb-8986-5589c67bb648.png)
  
2.Develop a program to perform Linear Transformation on image(Scaling and Rotation).
Scaling:
import cv2 
import numpy as np
img=cv2.imread('dog.jpg')
(height,width)=img.shape[:2]
res=cv2.resize(img, (int(width/2), int(height/2)), interpolation=cv2.INTER_CUBIC)
cv2.imwrite('result.jpg',res)
cv2.imshow('Result',res)
cv2.imshow('image',img)
cv2.waitKey(0)
cv2.destroyAllWindows()


  

  
