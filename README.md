# Dog Breed Classifier using CNN and transfer learning in Pytorch
# Project Overview
The goal of the project is to build a machine learning model that can be used within web app to process real-world, user-supplied images. The algorithm has to perform two tasks:

Given an image of a dog, the algorithm will identify an estimate of the canine’s breed.
If supplied an image of a human, the code will identify the resembling dog breed.
For performing this multiclass classification, we can use Convolutional Neural Network to solve the problem.The solution involves three steps. First, to detect human images, we can use existing algorithm like OpenCV’s implementation of Haar feature based cascade classifiers. Second, to detect dog-images we will use a pretrained VGG16 model. Finally, after the image is identified as dog/human, we can pass this image to an CNN model which will process the image and predict the breed that matches the best out of 133 breeds.
# Results

The CNN model created using transfer learning with ResNet101 architecture was trained for 10 epochs, and the final model produced an accuracy of 83% on test data. The model correctly predicted breeds for 697 images out of 836 total images.

Accuracy on test data: 83% (697/836)
