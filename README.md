# Image_Classification_MLP_PyTorch
Created an image classification model based on MLP (Multi Layer Perceptrons) for classifying images of Japanese Characters

The main objective of the project is to experiment with MLP's for image classification rather than CNN's. In most of the cases CNN's are better suited for the task of image classification since CNN's can better understand spatial relationships between pixels. However, in certain cases MLP's have been proved to give better results.

Information about dataset can be found at below link.
http://codh.rois.ac.jp/kmnist/index.html.en
![image](https://user-images.githubusercontent.com/102705658/230982773-cadcd5f6-207a-4945-9570-c7697dd63c12.png)


## Overview of Architecture

![image](https://user-images.githubusercontent.com/102705658/230982909-dc461661-ca08-4855-8443-14641df96471.png)

Where, 

       S- Stem

       B - Blocks (each block consisisting of two MLP's)
       
       c - Classifier
       
       
Multiple blocks joined together result in the backbone of the model. BAckbone takes input from Stem, processes it through multiple blocks and passes the output to the classifier.

