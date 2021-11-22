# Kaggle - Human Detection Net
## Description
You are given 3 sets of images: training (train), validation (valid) and test (test). Your task is to find on the test set which of the images contain people.

The markup is known for the training and validation sets. It is set in the train.csv and valid.csv files. Each of these files contains 2 columns:
id- the name of the file with the image
target_people - equal to 1 if the image contains at least one person and 0 if it does not.

The sample_submission.csv file contains a set of files with images located in the test folder, for which you need to predict the probability that people are present in the image.

## Data
train - folder with training images (9003 files)

valid - folder with validation images (1536 files)

test - folder with test images (4523 files)

train.csv - markup for training files

valid.csv markup for validation files

sample_submission.csv - sample file to send to the server

<a href="https://www.kaggle.com/c/mipt-x5-lab-2-run-2/data">Data</a>

## Solution
The idea of the solution is to retrain the ResNet50 neural network. The model is supplemented with linear layers and Relu layers. Score on the validation sample - 0.9063
Score on a private leaderboard - 0.90723

<img width="1215" alt="Training epochs info" src="https://user-images.githubusercontent.com/45330067/142923114-2183de89-8b40-4fcd-b6c5-3a2e939c6a92.png">

## Reference
<a href="kaggle.com/c/mipt-x5-lab-2-run-2">MIPT-X5 LAB 2</a>
