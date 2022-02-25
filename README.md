# Emotion-Detection

## Introduction

This Project aims to classify the emotion on a person's face into one of the **seven categories**, using deep convolution neural networks.
The **seven emotions** are angry, disgusted, fearful, happy, neutral, sad and suprised

## Dataset

This model is trained on the **FER-2013** dataset which was published on International Conference on Machine Learning (ICML). This dataset consists of 35887 grayscale, 48x48 sized face images 

you can download the FER-2013 dataset from here[https://www.kaggle.com/msambare/fer2013]


## Dependencies

- Python3, OPenCV, Tensorflow
- To install the required packages, run `pip install -r requirements.txt`.

## Algorithm


* First, the **haar cascade** method is used to detect faces in each frame of the webcam feed.

* The region of image containing the face is resized to **48x48** and is passed as input to the CNN.

* The network outputs a list of **softmax scores** for the seven classes of emotions.

* The emotion with maximum score is displayed on the screen


## Results

-  This implementation by default detects emotions on all faces in the webcam feed. With a simple 4-layer CNN, the test accuracy    reached 89.2% in 50 epochs.

- This model can detect multiple facial expressions in one images


<p align="center">
  <img width="1000" src="emoition_detection.png">
</p>

