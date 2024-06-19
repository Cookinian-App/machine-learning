# MACHINE LEARNING

## Overview

The Machine Learning part of this application is the recommendation system. We modeled an article recommendation system that classifies topics related to cooking, cooking tutorials, and health. The object that is scanned by the user is sent to the mobile and displays the cooking ingredients. After that, based on what the user has scanned, the model will recommend cooking categories that match the ingredients.

## Datasets

The dataset we use comes from [Roboflow][https://app.roboflow.com/ingridients/ingridients_detection/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true] and scraping images from Microsoft Edge and photographing the objects themselves using a cellphone camera. We collected 5200 images, of which 400 images per class with a total of 13 classes.

We annotate the dataset according to the name of each object. After annotating, we export the dataset into .tfrecord format.
For more details visit [datasets][https://github.com/Cookinian-App/machine-learning].

## Model Architecture

The model only achieved a loss of 0.37905806 on the training data. While in the roboflow data, the model achieved a loss of 0.539.

<details>
<summary>Model Accuracy & Loss</summary>

![model-loss](https://drive.google.com/file/d/1y-AL6S6Itl-8gttA0v2UeWYyJa41a3G9/view?usp=sharing)
![model-loss](https://drive.google.com/file/d/1iht-Sr-9bMuIvB1TaodGOLtMzi3roxdR/view?usp=sharing)

</details>

## How to replicate our projects

### 01 Data Preprocessing

To run this model you need to follow these steps:

- Download the datasets [here][https://github.com/Cookinian-App/machine-learning/tree/main/dataset]
- Upload the dataset in your notebook environment
- Install the required libraries
- Pre-process the data

### 02 Modelling

- Build and compile models with tflite architecture with metadata
- Do a model evaluation
- Convert the model to `.tflite` format the model result [here][https://github.com/Cookinian-App/machine-learning/blob/main/model/modelv4_128_optimize.tflite]

