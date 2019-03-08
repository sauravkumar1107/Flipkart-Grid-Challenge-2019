# Flipkart Grid Challenge 2019
The challenge was to predict the bounding box across the object in the image. We were given an image dataset including 56,791 images and two csv files. One was for training and another was for testing. Training csv file included the name e.g. "JPEG_20160706_121146_1000145715002.png" of 24k images and their corresponding coordinates of x1,x2,y1,y2. In testing csv file we were given the name of the 25k images and we had to predict the values of x1,x2,y1,y2 for the object in each image.

# Steps
1.	First I separated the training and test images from the image dataset and saved them into the memory. 
2.	Then I read each image of the training images as grayscale and appended this numpy array into a list and finally converted this list       into an array of size (24000, 480, 640, 1).
3.  Made an image data generator and applied feature center and std normalization.
4.	Created the CNN model and trained it using fit_generator and saved these weights into the memory
5.	Got the predictions on test images and made the csv file

# Libraries Used
Numpy, pandas, Keras, tensorflow, os, OpenCV, matplotlib, pickle

