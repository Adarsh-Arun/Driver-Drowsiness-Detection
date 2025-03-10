# Driver_drowsiness_system_CNN
This is a system that can detect the drowsiness of the driver using CNN - Python, OpenCV

The aim of this is a system to reduce the number of accidents on the road by detecting the drowsiness of the driver and warning them using an alarm. 

Here, we used Python, OpenCV, and Keras(Tensorflow) to build a system that can detect features from the faces of the drivers and alert them if ever they fall asleep while while driving. The system detects the eyes and prompts if it is closed or open. If the eyes are closed for 3 seconds it will play the alarm to get the driver's attention, to stop cause it's drowsy. We have build a CNN network which is trained on a dataset that can detect closed and open eyes. Then OpenCV is used to get the live feed from the camera and run that frame through the CNN model to process it and classify whether it opened or closed eyes.

## Setup
To set the model up:<br />
Pre-install all the required libraries <br />1) OpenCV<br />
                                       2) Keras<br />
                                       3) Numpy<br />
                                       4) Pandas<br />
                                       5) OS<br />
Could you download the dataset from the link below and edit the address in the notebook accordingly? <br />
Run the Jupyter Notebook and add the model name in the detect_drowsiness.py file in line 20.<br />

## The Dataset
The dataset that was used is a subnet of a dataset from(https://www.kaggle.com/datasets/dheerajperumandla/drowsiness-dataset)<br />
it has 4 folder which are <br />1) Closed_eyes - having 726 pictures<br />
                          2) Open_eyes - having 726 pictures<br />
                          3) Yawn - having 725 pictures<br />
                          4) no_yawn - having 723 pictures<br />

## The Convolution Neural Network
![CNN](https://user-images.githubusercontent.com/16632408/159187014-4bc4b70e-98d6-4313-873f-997ded2eff27.png)

## Accuracy 
We did 50 epochs, to get a good accuracy from the model i.e. 98% for training accuracy and 96% for validation accuracy.
![Graph](https://user-images.githubusercontent.com/16632408/159187004-92a72662-ddfe-471d-8bd6-65a3593a70a1.png)

## The Output 
1. Open Eyes<br />
![Open_eyes](https://github.com/Adarsh-Arun/requireq-files-and-photos/blob/main/Screenshot%20(352).png)
2. Close Eyes<br />
Here we detect whether the eyes are closed and count the number of frames for which the eyes were closed (10 frames) greater than that the Alarm will ring and the WARNING sign will be displayed.
![Closed_eyes](https://github.com/Adarsh-Arun/requireq-files-and-photos/blob/main/Screenshot%20(358).png)


