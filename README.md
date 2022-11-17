# Custom-object-detection:

## platform used: Google colab
## model -yolo version 4.
## dataset: custom dataset.
## labels: LCD, LED, Button.

# Project Description:
The model that is used for this project is darknet yolov4. This model will identifies the LCD, LED, Buttons in a panel. Moreover, it identifies the colour such as Green, Yellow and red and state such as on or off of the LED.

# Methodology: 
GPU is enabled in the colab and the datrkent is cloned from AlexyAB's repository. The configuration file is fine-tuned depending upon the problem.
## step1:
labeling images are manually done with the use of LabelImg software and saved them in yolo format.
## step2:
create two dataset folder namely train and validation folder.
Store the images to be trained and validated in their respective folders and their corresponding yolo format text files.
## step3:
move the dataset folder to cloud VM in zip file so that we can access it while training.
## step4:
create a folder yolov4 and save the compressed train and validation folder.
## step5:
Clone the darknet repo from AlexeyAB github profile.
## step6:
Unzip the train and validation folder in the data/darknet directory
## step7:
Change the configuration the yolov4 config file such as output layer, iteration, filters etc according to your application.
## step8:
Create a class file named train.names which includes labels such as LCD, LED, Button in my case.
## step9:
Create train.data file. this file is used to point the proper areas for all of the parameters. this file includes classes=3, train=path for train folder, valid-=path for validation folder,names=path for train.names, backup= path for backup folder that was created in the yolov4 Cloud VM folder. this backup folder is used to save the weights.
## step9:
Generate the text and train files which includes the path of the images to be trained and validated an save in data/darknet folder.


# Results:
![deva_prediction](https://user-images.githubusercontent.com/76246283/202581586-6de6ae0f-c517-4384-89a3-53d5fe8c136b.jpg)


https://user-images.githubusercontent.com/76246283/202580942-8ffba54d-7bde-4d3a-8b46-6192c14b4429.mp4


https://user-images.githubusercontent.com/76246283/202581298-658db9ea-0399-4515-9a4e-6ab156960525.mp4

# Credits:
https://www.youtube.com/watch?v=mmj3nxGT2YQ

