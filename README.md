# Face-Image-Detection
First of all make sure you have OpenCV installed. You can install it using pip:

pip install opencv-python

Face detection using Haar cascades is a machine learning based approach where a cascade function is trained with a set of input data. OpenCV already contains many pre-trained classifiers for face, eyes, smiles, etc.. Today we will be using the face classifier. You can experiment with other classifiers as well.

# Image Detection

* The detection works only on grayscale images.

* So it is important to convert the color image to grayscale.

* detectMultiScale function (line 10) is used to detect the faces.

* It takes 3 arguments — the input image, scaleFactor and minNeighbours.

* scaleFactor specifies how much the image size is reduced with each scale.

* minNeighbours specifies how many neighbors each candidate rectangle should have to retain it.

* You may have to tweak these values to get the best results.

* Faces contains a list of coordinates for the rectangular regions where faces were found.

* We use these coordinates to draw the rectangles in our image.

# Webcam Face Detection (For Video Detection also it has same description)

* Similarly, we can detect faces in videos. As you know videos are basically made up of frames, which are still images. 
* So we perform the face detection for each frame in a video.
* The only difference here is that we use an infinite loop to loop through each frame in the video.
* We use cap.read() to read each frame. The first value returned is a flag that indicates if the frame was read correctly or not. 
* We don’t need it. The second value returned is the still frame on which we will be performing the detection.

Github Repo Link:- https://github.com/srvjha/Face-Image-Detection
