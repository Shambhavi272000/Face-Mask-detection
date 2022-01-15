# Face-Mask-Detection-System
Created a face mask detection model using basics of machine learning.

## Algorithm Used:
> Voila Jones Object Detection Algorithm:
Developed in 2001 by Paul Viola and Michael Jones, the Viola-Jones algorithm is an object-recognition framework that allows the detection of image features in real-time.
Despite being an outdated framework, Viola-Jones is quite powerful and its application has proven to be exceptionally notable in real-time face detection.
1. How it works
There are 2 stages in the Viola-Jones Algorithm:
  > Training
  > Detection
    Training comes before detection, but for explanation’s sake, I’ll discuss detection first.
2. Detection
Viola-Jones was designed for frontal faces, so it is able to detect frontal the best rather than faces looking sideways, upwards or downwards. Before detecting a face, the image is converted into grayscale, since it is easier to work with and there’s lesser data to process. The Viola-Jones algorithm first detects the face on the grayscale image and then finds the location on the colored image.

Viola-Jones outlines a box (as you can see on the right) and searches for a face within the box. It is essentially searching for these haar-like features, which will be explained later. The box moves a step to the right after going through every tile in the picture. In this case, I’ve used a large box size and taken large steps for demonstration, but in general, you can change the box size and step size according to your needs.
With smaller steps, a number of boxes detect face-like features (Haar-like features) and the data of all of those boxes put together, helps the algorithm determine where the face is.
3. Haar-like Features
Haar-like features are named after Alfred Haar, a Hungarian mathematician in the 19th century who developed the concept of Haar wavelets (kind of like the ancestor of haar-like features). The features below show a box with a light side and a dark side, which is how the machine determines what the feature is. Sometimes one side will be lighter than the other, as in an edge of an eyebrow. Sometimes the middle portion may be shinier than the surrounding boxes, which can be interpreted as a nose.

There are 3 types of Haar-like features that Viola and Jones identified in their research:
Edge features
Line-features
Four-sided features

These features help the machine understand what the image is. Imagine what the edge of a table would look like on a b&w image. One side will be lighter than the other, creating that edge like b&w feature as you can see in the picture above.
In the two important features for Face Detection, the horizontal and the vertical features describe what eyebrows and the nose, respectively, look like to the machine.
Additionally, when the images are inspected, each feature has a value of its own.

In this work, a deep learning based model for detecting masks over faces in public place to curtail community spread of Coronavirus is presented. The proposed model efficiently handles varying kinds of occlusions in dense situation by making use of ensemble of single and two stage detectors. The ensemble approach not only helps in achieving high accuracy but also improves detection speed considerably. The model is 98.2% accurate at mask detection with average inference times of 0.05 seconds per image.

## What is facemak Detection 
The high accuracy of model is also due to highly balanced face mask centric dataset achieved through Random over-sampling with data augmentation over original MAFA dataset. Our technique reduces the imbalance ratio ρ = 11.82 (original) to ρ = 1.07.

## About Classification Algorithm:
> The Classification algorithm is a Supervised Learning technique that is used to identify the category of new observations on the basis of training data. In Classification, a program learns from the given dataset or observations and then classifies new observation into a number of classes or groups. Such as, Yes or No, 0 or 1, Spam or Not Spam, cat or dog, etc. Classes can be called as targets/labels or categories.
