# Autonomous driving applications : Object detection and image segmentation
This is a major project in the domain of object detection, computer vision and neural networks, completed by me for academic, self-learning, and hobby purpose.
# Details about the Project :
This project started as a capstone project for a Deep learning specialization course on Convolutional Neural Networks by Andrew Ng.

# Steps in the Project:
this project contains 2 parts :
1) To build car detection system. <br />
2) image segmentation with Unet <br />

# PART 1 : Build the Car Dtection Sysytem with YOLO - bounding boxes.
# 1) Packages
# 2) Problem Statement
Here We want to work on a self-driving car. As a critical component of this project, we need to first build a car detection system. To collect data, we can mount a camera to the hood (meaning the front) of the car, which takes pictures of the road ahead every few seconds as we drive around.We need to gathered all these images into a folder and labelled them by drawing bounding boxes around every car we found. Data set is provided by drive.ai
# 3) YOLO
"You Only Look Once" (YOLO) is a popular algorithm because it achieves high accuracy while also being able to run in real time. This algorithm "only looks once" at the image in the sense that it requires only one forward propagation pass through the network to make predictions. After non-max suppression, it then outputs recognized objects together with the bounding boxes. <br />
3.1) Model Details <br />
3.2) Filtering with a Threshold on Class Scores <br />
3.3) Non-max Suppression <br />
3.4) iou <br />
3.5) YOLO Non-max Suppression <br />
3.6)  Wrapping Up the Filtering <br />
# 4) Test YOLO Pre-trained Model on Images 
4.1) Defining Classes, Anchors and Image Shape <br />
4.2) Loading a Pre-trained Model <br />
4.3) Convert Output of the Model to Usable Bounding Box Tensors <br />
4.4) Filtering Boxes <br />
4.5) Run the YOLO on an Image <br />
# 5) Summary for YOLO 
# 6) References

# PART 2 : Image segmentation with Unet.
# 1) - Packages
# 2) - Load and Split the Data
2.1) - Split Your Dataset into Unmasked and Masked Images <br />
2.2) - Preprocess Your Data
# 3) - U-Net
3.1) - Model Details <br />
3.2) - Encoder (Downsampling Block) <br />
3.2.1) - conv_block <br />
3.3) - Decoder (Upsampling Block) <br />
3.3.1) - upsampling_block <br />
3.4) - Build the Model <br />
3.4.1) - unet_model <br />
3.5) - Set Model Dimensions <br />
3.6) - Loss Function <br />
3.7) - Dataset Handling <br />
# 4) - Train the Model
4.1) - Create Predicted Masks <br />
4.2) - Plot Model Accuracy <br />
4.3) - Show Predictions <br />
