# [NASA Spacesuit Detection](https://www.topcoder.com/challenges/116fc3d9-a4e0-4a93-8ef1-a075ae16ee88?tab=details)

## OBJECTIVE

 Spacesuit has unique movement patterns that can be observed during spacewalks or Extravehicular Activities (EVA), and mobility assessments are needed to discern and mitigate suit injury risk. It is very difficult to measure spacesuit motion in uncontrolled environments such as training facilities, and a novel method is needed to quantify spacesuit motions from conventional and readily available video and photographs without requiring or needing motion capture cameras. 
 
 Once validated for the accuracy and reliability of the posture extractions, the selected system will be deployed to estimate the EVA postures in current and future missions and analog training events. The framework will be applicable to Neutral Buoyancy Lab (NBL) and Active Response Gravity Offload System (ARGOS) testing, which will help to optimize training procedures. Additionally, the winning solution will be tested and validated on video recordings collected during the next-generation spacesuit testing. 
 
 NASA is seeking novel solutions to label and identify spacesuit motions from conventional and readily available video and photographs to overcome current system limitations in terms of cost and training feasibility.

 The computer vision algorithms are expected to have the ability to:
 1. Detect spacesuits in a variety of environments and lightning conditions.
 2. Correctly discriminate between an “unsuited” person and a spacesuit.
 3. Robustly extract suit postures from images partially occluded.
 4. Capable of functioning with a single or multiple spacesuits.


 ## TASK

 1. to extract polygonal areas that represent spacesuits from photographs,
 2. to determine the coordinates (in 2D pixel space) of some predefined joints (like Right Shoulder Joint or Left Knee Joint) from photographs,
 3. to determine the coordinates (in 3D metric space) of joints from videos.

## DATA
 Follow this [TOPCODER LINK](https://www.topcoder.com/challenges/116fc3d9-a4e0-4a93-8ef1-a075ae16ee88?tab=details) for more information.

 ## NOTEBOOKS
 1. Object Detection Data Creation Script.ipynb
 ```CMD
 Create a dataset in the COCO required format for image segmentation
 ```
 2. Object Detection Model Training.ipynb
 ```CMD
 Train a pytorch transfer learning image segmentation model from a pre-trained COCO trained model on COCO to identify spacesuit images.(Object Detection)
 ```
 3. COCO_Image_Viewer.ipynb
 ```CMD
 View details about a COCO dataset and preview segmentations on annotated images
 ```
4. SpaceSuit Classification.ipynb
```CMD
Train a TF Keras RESNET transfer Learning model on image classification to classify segmented images are of spacesuit or not. (Binary Image CLassification)
```
5.Pose Estimation - Evaluation.ipynb
```CMD
Using GOOGLE movenet model to detect spacesuit poses.
```