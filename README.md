# Candid-Photo-detection

Description:
---
The main idea behind this project is to take candid photos from a video either through the webcam or a locally stored one. Alternatively it can also distinguish which photos are candid, removing the hassle of selecting which photos should be published.

Models/Languages/Libraries used:
---
- [Face Detection](https://docs.openvinotoolkit.org/latest/_models_intel_face_detection_adas_0001_description_face_detection_adas_0001.html)
- [Head Pose Estimation](https://docs.openvinotoolkit.org/latest/_models_intel_head_pose_estimation_adas_0001_description_head_pose_estimation_adas_0001.html)
- [Emotion Recognition](https://docs.openvinotoolkit.org/latest/_models_intel_emotions_recognition_retail_0003_description_emotions_recognition_retail_0003.html)

Referenced from the Intel OpenVino [Pretrained models](https://software.intel.com/en-us/openvino-toolkit/documentation/pretrained-models) list.

- Python
- OpenCV

Approach:
---
- Detect the faces in the video frames using the **Face detection** model.
- Check for the **head pose** and the **emotion involed** in the frame.
- Select the one with happy/suprise emotion. 
###### The emotion recognition model has a list of fully convolutional network for recognition of five emotions ('neutral', 'happy', 'sad', 'surprise', 'anger').

#### The overall workflow of Intel OpenVIno is mentioned [here](https://docs.openvinotoolkit.org/latest/_docs_IE_DG_Introduction.html).



