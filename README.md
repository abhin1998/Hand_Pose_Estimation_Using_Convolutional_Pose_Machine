# Hand_Pose_Estimation_Using_Convolutional_Pose_Machine
## OverView
Hand pose estimation is the task of finding the joints of the hand from an image or set of video frames.Hand pose estimation<br/>
Determine 3D locations of hand joints.<br/>
Pose estimation refers to computer vision techniques that detect human figures in images and video.

## Dependencies
Jupyter Notebook

### Packages
tensorflow<br/>
numpy<br/>
matplotlib<br/>
opencv<br/>
pickle<br/>
random<br/>
os<br/>
time


## Model
 ### Convolutional Pose Machine
<img src="Outputs/Screenshot_2020-10-05 1602 00134 pdf.png"> 

### Stage 1
With an image as input, the classifier produces P+1 belief maps, where P is the number of body joints whose locations we are required to predict and the +1 is for background class.

### Stage 2 to T
At any stage t, the input to the classifier is the belief maps from stage t-1 and new features extracted from the image. This enables the pose machines to refine the prediction at every stage.

## Noations
    x: image feature extractor for stage 1
    g: classifier
    x’: feature extractor for stages (≥2); same for all stages
    b: belief maps
    psi: converts belief maps into better features for next stage classifier
 
## Download models
Put downloaded models in the models/weights folder.<br/>
Body Pose Model<br/>
Hand Pose Model (.pkl)<br/>
Hand Pose Model (tf)
    
    
## Variation
    ### MULTI will show multiple stages output heatmaps and the final pose estimation simultaneously.
    ### SINGLE will only show the final pose estimation.
    ### HM will show each joint heatmap of last stage separately.







## Model Test
<img src="Outputs/Untitled111 (2).png"> 
<br/>
<br/>
<img src="Outputs/Untitleaad (2).jpg">
<br/>
<br/>
<img src="Outputs/Untitledss (2).png">        
 <br/>
 
## Code

https://drive.google.com/file/d/1km0CDrnuId0CjxFeIlcmgubdy1dGlXxh/view?usp=sharing
 
## Video
 
 https://drive.google.com/file/d/1TWBH1Hr7RjA9vvbdEeW7CHbnd7aB3Qt4/view?usp=drivesdk

## Presentation
 
 https://drive.google.com/file/d/1km0CDrnuId0CjxFeIlcmgubdy1dGlXxh/view?usp=sharing

