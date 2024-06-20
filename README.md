# Cookinian ML 🧑‍🍳

Cookinian is an AI-powered cooking app designed to enhance users' cooking skills and expand their culinary knowledge. Cookinian implements an object detection model to identify users' food ingredients. When users utilize the scan feature, the app returns an image with bounding boxes and detected ingredients. These detected ingredients are then sent to the API, which returns a list of matching recipes.

## Datasets

The dataset we used comes from:

1. Existing datasets on Roboflow.
2. Scraping images from Bing Image and Google Search.
3. Our own photos taken with a cellphone camera.

For more details, visit our [datasets documentation](https://github.com/Cookinian-App/machine-learning/tree/main/dataset/readme.md).

## Model Architecture

![model-loss](https://raw.githubusercontent.com/Cookinian-App/machine-learning/main/docs/graph.png)

## Model Documentation

### Data Preprocessing

To run this model, follow these steps:

- Download the datasets. The dataset can be found [here](https://github.com/Cookinian-App/machine-learning/tree/main/dataset/readme.md).
- Upload the dataset to your notebook environment.
- Install the required libraries.
- Pre-process the data.

### Modelling

- Build and compile models with TensorFlow Lite architecture with metadata.
- Perform model evaluation.
- Convert the model to `.tflite` format.
- Add metadata to the model.
