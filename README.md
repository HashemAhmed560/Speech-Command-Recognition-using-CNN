# Speech-Command-Recognition-using-ANNs
The goal is to build a multiclass classification model using a Convolutional Neural Network (CNN) to recognize spoken commands. This model will classify short audio clips into specific commands from 0 to 1.
Speech Recognition Using Convolutional Neural Networks
Project Objective
The objective of this project is to build a deep learning model for speech recognition using Convolutional Neural Networks (CNN). The model will be trained to classify audio samples into different speech categories.
Dataset Information and Preprocessing
The dataset used for this project contains 23,666 audio samples across 10 different speech categories. The audio files were preprocessed as follows:

Data Loading: The audio files were loaded from the assignment data folder, with each subfolder representing a different speech category.
MFCC Extraction: The Mel-Frequency Cepstral Coefficients (MFCC) were extracted from each audio sample using the librosa library. This is a commonly used feature representation for speech recognition tasks.
Data Augmentation: To increase the size and diversity of the training data, background noise was added to the audio samples using the add_background_noise function.
Data Normalization: The MFCC features were normalized to have zero mean and unit variance using the normalize_mfcc function.
Data Splitting: The dataset was split into training and testing sets using the train_test_split function from sklearn.

Instructions for Running the Code

Ensure you have the following dependencies installed:

Python 3.x
numpy
librosa
scikit-learn
tensorflow
tqdm


Clone the repository and navigate to the project directory.
Open the Assignment.ipynb Jupyter Notebook file.
Run the cells in the notebook sequentially to load the data, preprocess it, define and train the CNN model, and evaluate its performance on the test set.

Dependencies and Installation
The project has the following dependencies:

numpy
librosa
scikit-learn
tensorflow
tqdm

You can install the required dependencies using pip:
Copypip install numpy librosa scikit-learn tensorflow tqdm
Alternatively, you can create a new virtual environment and install the dependencies using the provided requirements.txt file:
Copypython -m venv env
source env/bin/activate
pip install -r requirements.txt
Once the dependencies are installed, you can run the Jupyter Notebook as described in the "Instructions for Running the Code" section.
