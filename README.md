# Lip-Reader-Using-3DCNN

## Dataset:
The dataset for this can be found at this google drive link 'https://drive.google.com/uc?id=1YlvpDLix3S-U8fd-gqRwPcWXAXm8JwjL'.

## Introduction:
This is a Deep Learning Model used to generate transcipts just from observing the Lip movements of the mouth in the Video. 
The Project is a replication of a research paper, the link of which, I have provided below with some minor changes to the model.

## Methodology
First off we extract the face from the Video, this is done using the Dlib Face Detector from the Dlib Library. 
Next the Lip region is identified from the Face, as the Dlib Face Detector identifies faces using 68 points of interest to identify faces
,these points of interest can then be localised to get the Lip region. 
Next the frames are cropped around the lip region and then resized to get a uniform shape of the Frame.
Finally the frames are Passed into a 3D-CNN Deep Neural Network to train the model.

## Referenecs:
1. https://www.youtube.com/watch?v=uKyojQjbx4c (A video from Nicholas Renotte which was the basic inspiration)
2. https://arxiv.org/abs/1611.01599 (The Research Paper)
3. https://github.com/nicknochnack/LipNet/blob/main/LipNet.ipynb (Code for Reference in case of problems)
4. https://github.com/skaws2003/Dlib-lip-detection (The Dlib Face Detector)
