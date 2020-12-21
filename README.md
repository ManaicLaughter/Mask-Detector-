# Mask-Detector
Real-time COVID-19 face mask detector with OpenCV.

## Face Detection Algorithm
One of the popular algorithms that use a feature-based approach is the Viola-Jones algorithm.

Viola-Jones algorithm is named after two computer vision researchers who proposed the method in 2001, Paul Viola and Michael Jones in their paper, “Rapid Object Detection using a Boosted Cascade of Simple Features”. Despite being an outdated framework, Viola-Jones is quite powerful, and its application has proven to be exceptionally notable in real-time face detection. This algorithm is painfully slow to train but can detect faces in real-time with impressive speed.

Given an image(this algorithm works on grayscale image), the algorithm looks at many smaller subregions and tries to find a face by looking for specific features in each subregion. It needs to check many different positions and scales because an image can contain many faces of various sizes. Viola and Jones used Haar-like features to detect faces in this algorithm.
## Face Detection using OpenCV
I am going to use OpenCV to do real-time face detection from a live stream via our webcam.

As you know videos are basically made up of frames, which are still images. I perform the face detection for each frame in a video. So when it comes to detecting a face in still image and detecting a face in a real-time video stream, there is not much difference between them.

I will be using Haar Cascade algorithm, also known as Voila-Jones algorithm to detect faces. It is basically a machine learning object detection algorithm which is used to identify objects in an image or video. In OpenCV, we have several trained  Haar Cascade models which are saved as XML files. Instead of creating and training the model from scratch, we use this file.
