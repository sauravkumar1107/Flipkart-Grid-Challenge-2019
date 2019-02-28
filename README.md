# Flipkart Grid Challenge 2019
1.	First we separated the training and test images from the image dataset and saved them into the memory. 
2.	Then we read each image of the training images as grayscale and appended this numpy array into a list and finally converted this list     into an array of size (24000, 480, 640, 1).
3.	We made a image data generator and applied feature center and std normalization.
4.	Created the CNN model and trained it using fit_generator and saved these weights into the memory
5.	Get the predictions on test images and make the csv file
