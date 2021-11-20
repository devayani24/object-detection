# Custom-object-detection:
## platform used: Google colab
## model -yolo version 4.
## dataset: custom dataset.
## labels: LCD, LED, Button.
## step1:
### labeling images are done in LabelImg and save them in yolo format.
## step2:
### create two dataset folder namely train and validation folder.
### store the images to be trained and validated in their respective folders and their corresponding yolo format text files.
## step3:
### move the dataset folder to cloud VM in zip file so that we can access it while training.
## step4:
### create a folder yolov4 and save the compressed train and validation folder.
## step5:
### clone the darknet repo from AlexeyAB github profile.
## step6:
### unzip the train and validation folder in the data/darknet directory
## step7:
### change the configuration the yolov4 config file such as output layer, iteration, filters etc according to your application.
## step8:
### create a class file named train.names which includes labels such as LCD, LED, Button in my case.
## step9:
### create train.data file. this file is used to point the proper areas for all of the parameters. this file includes classes=3, train=path for train folder, valid-=path for validation folder,names=path for train.names, backup= path for backup folder that was created in the yolov4 Cloud VM folder. this backup folder is used to save the weights.
## step9:
### generate the text and train files which includes the path of the images to be trained and validated an save in data/darknet folder.
