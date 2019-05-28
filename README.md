# Binary-8-DataSet
This is the DataSet with training data and test data for the LightWeight CNN 'Binary-8' proposed to be used for ball detection on NAO robot. The dataset was collected in real RoboCup competitions and in TJArk lab, Tongji University, which consists of 1008 unique images with ball for training and 99 pictures for testing. In addition, the original images captured from the NAO’s cameras is YUV format and the size of the images are lowered to 640×480 pixels and 320×240 pixels from the upper and lower camera, respectively. In order to speed up the operation process and improve the robustness under various scenarios, only the luminance (Y) channel of each image was extracted from NAO in action with various light conditions. Only when the original dataset obtained, were the ball pixels manually labelled.

Note in the Folder of Training DataSet:

1. Train.txt and val.txt files placed in 'Training DataSet/ImageSets/Main/' write the absolute path of the training image for the model.
2. The folder JPEGImages stores all the original training images, total of 1008 pictures. And the folder 'labels' stores the corresponding label files. The details in the files descirbe the information of labeled ball box,'(classid, x, y, w, h)', and (x, y) corresponds to the coordinates of the box center point.
