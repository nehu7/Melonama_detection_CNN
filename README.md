# Melanoma Detection

## Introduction
> Melanoma is a skin cancer disease which is caused by changes in the properties of normal skin cells to become infectious, in which cells will continue to divide into abnormal shapes that are uncontrolled due to DNA damage. It can be deadly if not detected early. It accounts for 75% of skin cancer deaths. The objective is to build a CNN based model which can accurately detect melanoma. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

> The following types of skin cancer diseases are present in the dataset : actinic keratosis, basal cell carcinoma, dermatofibroma, melanoma, nevus, pigmented benign keratosis, seborrheic keratosis, squamous cell carcinoma, vascular lesion

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Model building](#Model-building)
* [Acknowledgements](#acknowledgements)

## General Information
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths.
A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Model building
- The entire code is divided into three parts-
* **Model 1 :** A baseline model which will try to learn from the images present in the dataset.
* **Model 2 :** To prevent overfitting of the model, dropdouts are added after each convolution+pooling layer
* **Model 3 :** Due to limited number of training images, the model doesn't generalize well. Used the Augmentor library to create transformations of train dataset with each class containing 500 images.

## Technologies Used
- pathlib
- tensorflow as tf
- matplotlib.pyplot as plt
- numpy as np
- pandas as pd
- matplotlib.pyplot as plt
- os
- PIL
- PIL.Image
- from tensorflow keras
- from tensorflow.keras.layers Rescaling, Conv2D, MaxPooling2D, Dense, Dropout, Flatten, Activation, BatchNormalization, RandomFlip, RandomRotation, RandomZoom
- from tensorflow.keras.utils image_dataset_from_directory

## Acknowledgements
- The final model is able to learn from the augmented images with an improved accuracy.
- This project was based on [this tutorial](https://learn.upgrad.com/course/1992/segment/12362/126148/385960/2008503).

## Contact
Created by [@nehu7] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
