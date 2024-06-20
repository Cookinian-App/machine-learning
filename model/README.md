# Cookinian ML 🧑‍🍳

## Our Notebook

We use two different environments to run our notebooks.

### Main Environment

Our main environment is used by `training.ipynb` and `optimize_saved_model.ipynb`. These notebooks are run on **Kaggle**. All necessary dependencies are compatible with the **Kaggle** environment. Any custom dependencies we use are included within the notebook using `!pip` cells.

### Additional Environment

We require a specific environment to run the `adding_metadata.ipynb` notebook. This environment is set up in **Anaconda**. The dependencies are:
- **`python`** == 3.8.0
- **`tensorflow`** == 2.4.0
- **`tflite-support`** == 0.3.1

Additionally, we use **Jupyter Notebook** as the code editor on this environment.
