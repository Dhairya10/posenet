# PoseNet

## Project Overview
This project uses the PoseNet model for pose estimation on an Android application.

The app uses the front camera of the mobile phone and estimates the pose of the driver sitting inside the car.
A score is generated based on the visibility and confidence of the keypoints.

![Screenshot 2020-10-20 at 2 32 17 PM](https://user-images.githubusercontent.com/36099337/96565209-b6474e00-12e1-11eb-93a1-5d28978e98f7.png =250x)

Working of the app can be seen [here](https://youtu.be/3DU02xnbQV8).

## PoseNet Model

The PoseNet model estimates the pose based on the presence/absence of keypoints. The keypoints used in this example are as follows.

    NOSE,  
    LEFT_EYE,  
    RIGHT_EYE,  
    LEFT_EAR,  
    RIGHT_EAR,  
    LEFT_SHOULDER,  
    RIGHT_SHOULDER,  
    LEFT_ELBOW,  
    RIGHT_ELBOW

A keypoint confidence score is returned for each keypoint and its average is taken as the final score.

## References

https://github.com/tensorflow/examples/tree/master/lite/examples/posenet/android
