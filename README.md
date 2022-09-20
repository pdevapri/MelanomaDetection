# Project Name
> Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. We are required to build a CNN based model which can accurately detect melanoma.  A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Steps Followed](#steps-followed)
* [Conclusions](#conclusions)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
- We are required to build a CNN based model which can accurately detect melanoma. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- The data set contains the following diseases-
     Actinic keratosis,
     Basal cell carcinoma,
     Dermatofibroma,
     Melanoma,
     Nevus,
     Pigmented benign keratosis,
     Seborrheic keratosis,
     Squamous cell carcinoma,
     Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Steps Followed
- Data Reading/Data Understanding: Defining the path for train and test images. 
- Dataset Creation: Creating train & validation dataset from the train directory with a batch size of 32. Resized images to 180*180.
- Dataset visualisation: Visualize 1 instance of all the nine classes present in the dataset.
- Model Building & training : Build a CNN model, which can accurately detect 9 classes present in the dataset. Images are rescaled and normalize pixel values between (0,1).
- Model Builing using manual augmentation : Model Building & training on the augmented data.
- Class distribution: Which class has the least number of sampled and which class  dominate the data.
- Model Building using  Augmentor library: Model Building & training on the rectified class imbalance data.

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Conclusions
- Model 1 is highly overfitting
- Model 2 with manual augmentation didn’t have major impact on the overfitting . however there is a very minimal improvement . The difference between the training and validation accuracy has reduced
- Model 3 with augmentor library , the overfitting has reduced to a vast extend.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->
