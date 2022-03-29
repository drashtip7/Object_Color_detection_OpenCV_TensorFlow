The problem is divided into two parts :  1. Object detection   2. Color recognition

1.Object detection  - Detecting the vehicle:

  * For Object detection i have used Pre-trained Cascade classifier

2.Color recognition - Recognizing the color of the vehicle.

Performed steps:
------------------
   1. Feature Extraction:
       > Perform feature extraction for getting the R, G, B Color Histogram values of training images
   2. Training K-Nearest Neighbors Classifier:
       > Train KNN classifier by R, G, B Color Histogram values
   3. Classifying by Trained KNN:
       > Read video frame by frame, perform feature extraction on each frame and then classify the mean color of it by trained KNN classifier.

In this project :
--------------------

1.) Feature Extraction = Color Histogram

* Color Histogram is a representation of the distribution of colors in an image. For digital images, a color histogram represents the number of pixels that have colors in each of a fixed list of color ranges,  that span the image's color space, the set of all possible colors.

2.) Classification = K-Nearest Neighbors Algorithm

* K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure.

This K-Nearest Neighbors algorithm includes :
                             1. Fetching training data
                             2. Fetching test image features
                             3. Calculating euclidean distance
                             4. Getting k nearest neighbors
                             5. Prediction of color
                             6. Returning the prediction is true or false

