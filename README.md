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

The images in original folder named 'images' are managed to be in the file structure to be able to work with Keras ImageDataGenerator object as in folder name 'dataset'.  
The process of preparation is included in the notebook.  

## Model Development (are performed on Google COLAB)
The models used in this multiclass classification problem are  
- simple CNN
- NN with VGG blocks 
- NN with Keras pre-trained VGG16 as a feature extractor 
- NN with Keras pre-trained ResNet50 as a feature extractor 

## Prediction
The best model from above are selected and make a prediction.  
There are both prediction of one image and several images (batch) at a time.
