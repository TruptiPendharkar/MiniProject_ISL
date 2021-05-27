# MiniProject_ISL
### Real Time ISL prediction

### We have done this project in our 5th semester (Aug 2020- December 2020)


###  <p align="center">METHODOLOGY</p>

## <p align="center">1. Dataset Generation:</p>
  
As less research has been done for the Indian Sign Language as compared to ASL proper dataset
is not available for ISL, so we have prepared our own dataset. We have built a python file
through which we can generate our data for all the Classes. So for creating a dataset we have to
use the Open Computer Vision(OpenCV) library. Firstly we captured around 7000 total images
200 for each 35 labels ISL. Then we divided the dataset in 80:20 percent ratio into training and
testing data respectively.


##### <p align="center">All Gestures</p>            
   &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; ![All gestures](all_gestures.jpg) 



### <p align="center">2.  Image Preprocessing</p>

### Image Segmentation:

The goal of Image segmentation is to remove background and noises or we can say simplify
and/or change the representation of an image into something which is Region of Interest (ROI)
and the only useful information in the image. Image segmentation is typically used to locate
objects and boundaries (lines, curves, etc.) in images.

Two Basic Steps for image segmentation performed are:

##### <p align="center">1. Skin Masking :</p>
Using the concept of thresholding this RGB color space is converted into
grayscale image and SkinMask is finally obtained through HSV color space(which we get
from gray scale image)

##### <p align="center"> Raw Image for Letter A</p>
   &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp;  ![Raw Image for letter A](rawimageA.jpg)
	 
<h1 align="center">  &#8659;</h1>

##### <p align="center"> Gray Scale Image for letter A</p>
   &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp;  ![Gray Scale Image for letter A](skin.jpg)
	 
<h1 align="center">  &#8659;</h1>

##### <p align="center"> Skin Mask for letter A</p>
   &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp;  ![Skin Mask Image for letter A](skinmaskA.jpg)
	 
<h1 align="center"> &#8659;</h1>

#####  2. Canny Edge Detection:
It is basically a technique which identifies or detects the presence of
sharp discontinuities in an image there by detecting the edges of the figure in focus.

##### &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp;  &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; Skin Mask for letter A                                         
   &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp;  ![Skin Mask Image for letter A](skinmaskA.jpg)	
   
 <h1 align="center">  &#8659;</h1>

##### &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp;  &ensp; &ensp; Edge Detected(Canny Edge detection) Image for letter A
   &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; ![Edge Detected Image for letter A](cannyA.jpg)
   

### Feature Extraction:

#### 1. Feature Detection

key features of the image were extracted using SURF technique.
SURF is a feature extraction algorithm which is robust against rotation variation scaling.
We have extracted features using the inbuilt SURF function in opencv.










