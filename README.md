# Darkflow-Object-Identification-Tunnel-
Using Darkflow, to implement the Yolo algorithm to identify objects in images of the interior of a tunnel created from point cloud data

## Abstract
LiDAR scans capture minute details of the boundaries and the surface of a structure. It generates huge amounts of point cloud information which when processed and analyzed can show interesting features and generate 3D digital models of the structure. A large amount of point cloud data was generated of a LiDAR scan taken of a tunnel.
The overall purpose if this project was to identify the locations of different materials in this tunnel using the point cloud data. The point cloud data was converted into images which were used for object detection. We used the state of the art YOLOv2 algorithm to carry out object detection to identify the objects of interest. Our project shows that the algorithm can detect most objects of interest, with confidence going up to 0.80, however it does not necessarily identify all the instances of the objects. Some overlapping objects are identified with high confidence but the generated bounding boxes are not accurate.

## This repository includes:
1. Images for training
2. Annotations for all the training images
3. Test images with "out" directory containing the test results
4. Report on project
5. Darkflow code 
6. Python code - yolov_train_ritika, yolo_test_ritika                                       

### Pre-requisites to run the code:
1. Python3, Tensorflow, Numpy , OpenCV, Matplotlib, Cython

### Steps to run the code
A) FROM THIS REPOSITORY
1. Git clone this repository
2. Navigate to Darkflow folder. You should be able to see setup.py file.
   According to the darflow author thtrieu, you need to  build the Cython extensions. In order to do so, in the darkflow directory run      the    following command 'python setup.py build_ext --inplace'. You will be able to see installations in the cython_utils directory      as well as    in your site-packages.
3. To use the weights that I have trained (RECOMMENDED), download the ckpt folder https://drive.google.com/open?id=1koylWjEUJtwyaZoIDFC-    zqPb54XFWsb4  and place it in the darkflow folder. I have set up the code in such a way that it uses the latest checkpoint i.e 96876    to make predictions as well as continue training.  If you want to train the model from scratch , download the bin folder from here -    and place it in the darkflow folder. You will have to make the necessary changes in the code to use these weights instead. (Explained    in the comments in ipnyb files mentioned below.
2. There are two more files in this directory 1)yolo_train_ritika and 2) yolo_test_ritika
3. If you want to visualize the results , open up yolo_test_ritika.ipnyb.  
4. Run the jupyter notebook.

B) FROM THE ZIP FILE NAMED "DATS 6501 - Capstone Project - Ritika Agarwal"
1. Navigate to Darkflow folder with setup.py
2. According to the darflow author thtrieu, you need to  build the Cython extensions. In order to do so, in the darkflow directory run      the    following command 'python setup.py build_ext --inplace'. You will be able to see installations in the cython_utils directory.
3. There are two more files in this directory 1)yolo_train_ritika and 2) yolo_test_ritika
4. If you want to visualize the results , open up yolo_test_ritika.ipnyb.  
5. Run the jupyter notebook.
 
 

