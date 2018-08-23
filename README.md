# Image Classification of Furniture and Home Goods using Imaterialist data
Identify non-cluttered images and classify using Keras, TF and Object Detection API

# Environment setup:
Anaconda3, Python 3.6, TensorFlow CPU(1.8.0), Keras 2.2.0, OpenCV, PILLOW

# JSON:
To download train, validation and test images from JSON provided in iMaterialist Furniture Challenge
https://www.kaggle.com/c/imaterialist-challenge-furniture-2018

JSONs for train, validation and test are provided separately.

# Scripts:
1. DownloadImages.ipynb
    For downloading images in a multithreaded environment using the JSONs provided.
2. ImageNoise.ipynb
    If you are using a small subset of the images for training, this script will help in adding Gaussian Noise to the colored images.

# Algorithms:
1. FineTuned VGG16 Model  with ROC_AUC and Confusion Matrix.ipynb for training the model
2. Object_Detection_Algorithm for classifying good and bad images.ipynb - For segregating non-cluttered (good images) from cluttered (bad images) images. The good images from this algorithm serve as inputs to the FineTuned VGG16 Model.
3. Algo2_Predictor_for_new_test_images.ipynb for predicting the categories for new images


# Credits
This is an extension to the code provided by https://gist.github.com/fchollet/7eb39b44eb9e16e59632d25fb3119975

