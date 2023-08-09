# Gesture Recognition Assignment

Developed by: Shashank Pawaskar (https://github.com/ShashankPawas)

### Problem Statement
Imagine you are working as a data scientist at a home electronics company which manufactures state of the art smart televisions. You want to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.

The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:
 
| Gesture | Corresponding Action |
| --- | --- | 
| Thumbs Up | Increase the volume. |
| Thumbs Down | Decrease the volume. |
| Left Swipe | 'Jump' backwards 10 seconds. |
| Right Swipe | 'Jump' forward 10 seconds. |
| Stop | Pause the movie. |

Each video is a sequence of 30 frames (or images).

### Objectives:
1. **Generator**:  The generator should be able to take a batch of videos as input without any error. Steps like cropping, resizing and normalization should be performed successfully.

2. **Model**: Develop a model that is able to train without any errors which will be judged on the total number of parameters (as the inference(prediction) time should be less) and the accuracy achieved. As suggested by Snehansu, start training on a small amount of data and then proceed further.

3. **Write up**: This should contain the detailed procedure followed in choosing the final model. The write up should start with the reason for choosing the base model, then highlight the reasons and metrics taken into consideration to modify and experiment to arrive at the final model.

### Dataset:
You can download the dataset from [here.](https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL)
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use. 

### Results:

Final Model Chosen is CNN2D+Conv2DLSTM2D based Model 6 as it has fairly decent accuracy considering the type of data (where Validation dataset is low in numbers) as well the no. of parameters and the requirement of the assignment is to have light weight model.

Following are l

![Final-Train-Val-Plots](https://github.com/ShashankPawas/Gesture-Recognition-Assignment/blob/main/Final-Train-Val-Plots/Conv2D-FinalModel-ResultPlot.PNG)

![Conv2DFinalModel-Architecture](https://github.com/ShashankPawas/Gesture-Recognition-Assignment/blob/main/Conv2DFinalModel-Architecture/CNN_2d_CLSTM_model_6.png)

H5 Files Link - https://github.com/ShashankPawas/Gesture-Recognition-Assignment/blob/main/H5%20Files/model-00039-0.33804-0.87351-0.34433-0.91071.h5
