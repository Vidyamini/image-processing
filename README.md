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

  

  

  