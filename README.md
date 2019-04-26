# Darkflow-Object-Identification-Tunnel-
Using Darkflow, to implement the Yolo algorithm to identify objects in images of the interior of a tunnel created from point cloud data

## Abstract
LiDAR scans capture minute details of (http://www.lidar-uk.com/usage-of-lidar/) the boundaries and the surface of a structure. It generates huge amounts of point cloud information which when processed and analyzed can show interesting features and generate 3D digital models of the structure. A large amount of point cloud data was generated of a LiDAR scan taken of a tunnel.
The overall purpose if this project was to identify the locations of different materials in this tunnel using the point cloud data. The point cloud data was converted into images which were used for object detection. We used the state of the art YOLOv2 algorithm to carry out object detection to identify the objects of interest. Our project shows that the algorithm can detect most objects of interest, with confidence going up to 0.80, however it does not necessarily identify all the instances of the objects. Some overlapping objects are identified with high confidence but the generated bounding boxes are not accurate.

## This repository includes:
1. Images for training
2. Annotations for all the training images
3. Test images with "out" directory containing the test results
4. Report on project
5. Darkflow code 
6. Python code - yolov_train_ritika, yolo_test_ritika                                       

### Pre-requisites to run the code:
1. Python3, Tensorflow, Numpy , OpenCV, Matplotlib

### Steps to run the code
1. Git clone this repository
2. Start jupyter notebook in the directory "Darkflow_Object_Identification_Capstone"
3. The above directory should be your current working directory
4. There are two files 1)yolo_train_ritika and 2) yolo_test_ritika
5. If you want to visualize the results , open up yolo_test_ritika.ipnyb. 
6. Run the jupyter notebook.
  a. If you 
 

