# Mask-Detector
Real-time COVID-19 face mask detector with OpenCV using just a single image instead of large datasets.

## Face Detection Algorithm
One of the popular algorithms that use a feature-based approach is the Viola-Jones algorithm.

Viola-Jones algorithm is named after two computer vision researchers who proposed the method in 2001, Paul Viola and Michael Jones in their paper, “Rapid Object Detection using a Boosted Cascade of Simple Features”. Despite being an outdated framework, Viola-Jones is quite powerful, and its application has proven to be exceptionally notable in real-time face detection. This algorithm is painfully slow to train but can detect faces in real-time with impressive speed.

Given an image(this algorithm works on grayscale image), the algorithm looks at many smaller subregions and tries to find a face by looking for specific features in each subregion. It needs to check many different positions and scales because an image can contain many faces of various sizes. Viola and Jones used Haar-like features to detect faces in this algorithm.

## Face Detection using OpenCV
I am going to use OpenCV to do real-time face detection from a live stream via my webcam.

As you know videos are basically made up of frames, which are still images. I perform the face detection for each frame in a video. So when it comes to detecting a face in still image and detecting a face in a real-time video stream, there is not much difference between them.

I will be using a reference image to detect mask in real time video stream. It is basically a machine learning object detection algorithm which is used to identify objects in an image or video. In OpenCV, we have several trained Haar Cascade models which are saved as XML files. Instead of creating and training the model from scratch, I am using this reference image file.

This method haev less accuracy compared to algorithms trained using large datasets. But collecting data for creating dataset is really tough and it takes a lot of time to train the AI.

### Jugaad
So I came up with this juggad algorithm that can do mask detection using just a single reference image and the algorithm is ready in less then 10 mins to detect mask in Real-time.
