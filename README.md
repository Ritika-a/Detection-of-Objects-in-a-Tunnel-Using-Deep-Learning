# Detetction of Objects in a Tunnel Using Deep Learning
Using Darkflow, to implement the Yolo algorithm to identify objects in images of the interior of a tunnel created from point cloud data

### Abstract
LiDAR scans capture minute details of the boundaries and the surface of a structure. It generates huge amounts of point cloud information which when processed and analyzed can show interesting features and generate 3D digital models of the structure. A large amount of point cloud data was generated of a LiDAR scan taken of a tunnel.
The overall purpose if this project was to identify the locations of different materials in this tunnel using the point cloud data. The point cloud data was converted into images which were used for object detection. I used the state of the art YOLOv2 algorithm to carry out object detection to identify the objects of interest. My project shows that the algorithm can detect most objects of interest, with confidence going up to 0.80, however it does not necessarily identify all the instances of the objects. Some overlapping objects are identified with high confidence but the generated bounding boxes are not accurate.

### This repository includes:
1. Report on project
2. Darkflow code 
3. Python code for training and testing- yolo_train_ritika, yolo_test_ritika
                                        

### Pre-requisites to run the code:
1. Python3, Tensorflow, Numpy-1.16.3 , OpenCV(opencv-python), Matplotlib, Cython

### Steps to run the code

A)FROM THIS REPOSITORY - I have not uploaded the images or labels for training the data. 
To  run the darkflow code for your own dataset, you can got go to the official Darkflow page and follow the instructions given in the readme file. https://github.com/thtrieu/darkflow. I have additionally provided 2 ipnyb file, yolo_train_ritika and yolo_test_ritika to train as well as generate predictions for your own data. You can modify the paths for the images and annotations to point to your data and run the codes after setting up darkflow.

B) FROM THE ZIP FILE NAMED "DATS 6501 - Capstone Project - Ritika Agarwal"
1. Navigate to Darkflow_Object_detection_tunnel/Darkflow folder with the setup.py in it.
2. There are two more files in this directory 1)yolo_train_ritika and 2) yolo_test_ritika
3. If you want to visualize the results , open up yolo_test_ritika.ipnyb. Make sure that the darkflow directory where these files exist is your current working directory.
4. Run the jupyter notebook.
5. The test results, will be saved in a directory named "out" within the test_images directory. 
 
 Note:If there is an error saying that it cannot find cy_yolo_findboxes, then you shoudld do the following. According to the darflow author thtrieu, you need to  build the Cython extensions. In order to do so, in the darkflow directory (where setup.py exists) run the following command 'python setup.py build_ext --inplace' from your terminal/command prompt. You will be able to see installations in the cython_utils directory.
 
### References
 1. Thtrieu.(2017)- Darkflow code . https://github.com/thtrieu/darkflow 
 2. Tzutalin. LabelImg. Git code (2015). https://github.com/tzutalin/labelImg
 3. Lidar-UK Websites. Taken from http://www.lidar-uk.com/usage-of-lidar/
 4. Park Chansung. (2018) YOLOv2 to detect your own objects using Darkflow.  Taken from https://towardsdatascience.com/yolov2-to-      detect-your-own-objects-soccer-ball-using-darkflow-a4f98d5ce5bf
 
 

