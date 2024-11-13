# Speech-Command-Recognition-using-ANNs

## Project Objective
The goal is to build a multiclass classification model using a Convolutional Neural Network (CNN) to recognize spoken commands. This model will classify short audio clips into specific commands from 0 to 1.
## Dataset Information and Preprocessing
The dataset used for this project contains 23,666 audio samples across 10 different speech categories. The audio files were preprocessed as follows:
1.Data Loading: The audio files were loaded from the assignment data folder, with each subfolder representing a different speech category. <br>
2.MFCC Extraction: The Mel-Frequency Cepstral Coefficients (MFCC) were extracted from each audio sample using the librosa library. This is a commonly used feature representation for speech recognition tasks.<br>
3.Data Augmentation: To increase the size and diversity of the training data, background noise was added to the audio samples using the add_background_noise function.<br>
4.Data Normalization: The MFCC features were normalized to have zero mean and unit variance using the normalize_mfcc function.<br>
5.Data Splitting: The dataset was split into training and testing sets using the train_test_split function from sklearn.<br>

## Instructions for Running the Code<br>

1.Ensure you have the following dependencies installed:<br>
  Python 3.x<br>
  numpy<br>
  librosa<br>
  scikit-learn<br>
  tensorflow<br>
  tqdm<br>
  matplot<br>
  seaborn<br>

2.Clone the repository and navigate to the project directory.<br>
3.Open the Assignment.ipynb Jupyter Notebook file.<br>
4.download the dataset from Kaggle: https://www.kaggle.com/datasets/neehakurelli/google-speech-commands/data (download only the commands from 0 to 9) and edit the *data_folder* variable with the path where you downlaoded it. <br>
<br>
5.Run the cells in the notebook sequentially to load the data, preprocess it, define and train the CNN model, and evaluate its performance on the test set. <br>

## Dependencies Installation<br>
You can install the required dependencies using pip:<br>
ex:pip install numpy librosa scikit-learn tensorflow tqdm numpy seaborn matplotlib<br>
Once the dependencies are installed, you can run the Jupyter Notebook as described in the "Instructions for Running the Code" section.<br>
