# Garbage Image Classification

## Objective
To classify type of garbage in an image.  
This dataset contains 6 types of garbage;  
   cardboard (393 images)  
   glass (491 images)  
   metal (400 images)  
   paper (584 images)  
   plastic (472 images)  
   trash (127 images)  

## Dataset 
The dataset is collected from https://www.kaggle.com/asdasdasasdas/garbage-classification.  
The dataset is separated into train, validation and test sets as shown in these 3 files :
- one-indexed-files-notrash_train.txt
- one-indexed-files-notrash_val.txt
- one-indexed-files-notrash_test.txt
The images in original folder named 'images' are managed to be in the file structure to be able to work with Keras ImageDataGenerator object as in folder name 'data'.  
All process of this preparation is in 01_data_preparation.ipynb.

## Model Development (are performed on Google COLAB)
The models used in this multiclass classification problem are  
- simple CNN (developed in 02_simple_CNN.ipynb)
- NN with VGG blocks (developed in 03_VGG_blocks.ipynb)
- NN with Keras pre-trained VGG16 as a feature extractor (developed in 04_pretrained_VGG16.ipynb)
- NN with Keras pre-trained ResNet50 as a feature extractor (developed in 05_pretrained_ResNet50.ipynb)

## Prediction
The best model from above are selected and make a prediction.  
(Note : Need to get model.h5 from the selected model ipython notebook by running it first,  
or you can get my model .h5 files at the bottom of this README)
The prediction process is presented in 06_make_prediction.ipynb.  
There are both prediction of one image and several images (batch) at a time.

## My best trained models
- model with pretrained ResNet50 : https://drive.google.com/file/d/13AZ_KiVfI5IpTpWt_D0Zf_E0OSIE4rqJ/view?usp=sharing
## other trained models
- simple CNN model : https://drive.google.com/file/d/1--QGWjBmwef1DYaHOF0tvnQD9TTKwa6s/view?usp=sharing
- VGG blocks model : https://drive.google.com/file/d/1bLMOSJlz0zAyp2_0lWm7ecl_LjUZe-XT/view?usp=sharing
- model with pretrained VGG16 : https://drive.google.com/file/d/1QoCPfVF4_Zop4JEPvMZegcyETAA-eocE/view?usp=sharing
