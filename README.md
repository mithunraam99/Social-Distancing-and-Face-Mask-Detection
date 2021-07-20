# Social Distancing and Face Mask Detection

Social distance monitoring and face mask detection system using a deep learning model has been implemented to tackle COVID-19 situation. This has been achieved by using **YOLO v3** object detection method which detects the persons in the video sequences and by using **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise)clustering method which estimates the distance between persons. To help the training process, augmented masked faces were generated using facial landmarks and blurring effects were also added. Any non-compliant pair has been indicated with a red bounded box and a red line between them. Safe pair has been indicated with a green bounded box around them. **DFSD** face detection method has been used to detect whether the persons were wearing a mask or not. Green bounded box around the face has been used if the mask was on the face and the red bounded box around the face has been used if the mask wasn’t on the face.


## Dataset and Weights

Dataset and pretrained weights can be downloaded from the below link:
https://drive.google.com/drive/folders/1OB-Nf5s3etAQHeRG1YeatMNyfDRZDKK2

## Tools Used
* [NumPy](https://numpy.org/) : Used for storing and manipulating high dimensional arrays.
* [Matplotlib](https://matplotlib.org/) : Used for plotting.
* [Scikit-Learn](https://scikit-learn.org/stable/) : Used for DBSCAN clustering.
* [PIL](https://pillow.readthedocs.io/en/stable/) : Used for manipulating images.
* [OpenCV](https://opencv.org/) : Used for manipulating images and video streams.
* [Keras](https://keras.io/) : Used for designing and training the Face_Mask_Classifier model.
* [face-detection](https://github.com/hukkelas/DSFD-Pytorch-Inference) : Used for detecting faces with Dual Shot Face Detector.
* [face-recognition](https://github.com/ageitgey/face_recognition) : Used for detecting facial landmarks.

## Algorithms
* **YOLO** - Object Detection (Person)
* **DSFD** - Face Detection
* **DBSCAN** - Distance Calculation

## Future Work
* Speed Optimization
* Realtime monitoring in crowded places

## Results
![](Results/Sample_Result.gif)
