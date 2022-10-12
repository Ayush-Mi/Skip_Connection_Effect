# Effect of Skip Connections in Shallow Network

## Description
We all must have seen the effect of skip connection based network which outperforms the traditional CNN models when the network has many hidden layers. This repo is to observe the effect of skip connection over shallow network and how it performs as compared to the traditional CNN. 

The tests were performed on Mac-M1 with a memory of 32gb.


## Dependencies
All the required dependecies can be installed from requirement.txt file

## Dataset
The dataset used was [American Sign Language](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) taken from the kaggle. It contains the images of hand gestures for all the 26 alphabets in the English language.

## Models
The architecture of the both models is shown below. The number of CNN layers and the number of filters remains the same for both, howver in ResNet architecture there are two residual block whose outputs are added later in the network.

ResNet Model | CNN Model
:---: | :---:
![](https://github.com/Ayush-Mi/Skip_Connection_Effect_On_Shallow_Network/blob/main/result_image/tmp.png) | ![](https://github.com/Ayush-Mi/Skip_Connection_Effect_On_Shallow_Network/blob/main/result_image/cnn_connection.png)

## Results

CNN Model
Accuracy | Loss
:---: | :---:
![](https://github.com/Ayush-Mi/Skip_Connection_Effect_On_Shallow_Network/blob/main/result_image/cnn_accuracy_plot.png) | ![](https://github.com/Ayush-Mi/Skip_Connection_Effect_On_Shallow_Network/blob/main/result_image/cnn_loss_plot.png)

ResNet Model
Accuracy | Loss
:---: | :---:
![](https://github.com/Ayush-Mi/Skip_Connection_Effect_On_Shallow_Network/blob/main/result_image/skip_connection_accuracy_plot.png) | ![](https://github.com/Ayush-Mi/Skip_Connection_Effect_On_Shallow_Network/blob/main/result_image/skip_connection_loss_plot.png)

## Future Works
This can be expanded further to train deeper model and see the actual impact of skip connection method. However, if the dataset and number of classes is small then the traditional CNN networks are easier to train and converges faster.
