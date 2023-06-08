# BTP
Defect detection


In this project we have implemented three different methods for classifying the defect into one of the six classes and also find out the location of the defects by using three different methods.The dataset used for the project is NEU-DET for training and evaluating our method. It is taken from Northeastern University (NEU) surface defect database. It includes six kinds of typical surface defects of the hot-rolled steel strip collected, i.e. 1. crazing (Cr) 2. patches (Pa) 3. pitted surface (PS) 4. rolled-in scale (RS) 5. inclusion (In) 6. scratches (Sc). 

Now, we did Data Analysis and Data Pre-processing which includes data augmentation , resizing and adding blurred images.

CLASSIFICATION:

Using CNN , CNN with transfer learning(MobileNet and VGG)

CNN With Transfer Learning: We have tried multiple models using transfer learning techniques for
finding the best accuracy. These models are VGG16 and MobileNet.The best accuracy we got among
them is with MobileNet, around 99.72%.

LOCALIZATION: We have used three methods :

FPN with ResNet : FPN is a feature extractor used with a object detection model such as ResNest which is deep convolutional neural network architecture. It solves the problem of vanishing gradient.

Unet with ResNet as encoder: U-Net is a convolutional neural network (CNN) architecture. It consist of two parts encoder and decoder. The purpose of the encoder pathway is to extract high-level semantic information and capture global context from the input image. The decoder pathway aims to recover spatial details and localize objects accurately.

YOLO: YOLO divides the input image into a grid of cells, typically, for example, a 4x4 or 7x7 grid. Each grid cell is responsible for predicting bounding boxes and associated class probabilities for objects that are located within that cell.

The best accuracy we got using YOLO: 74%.
