# Computer-Aided Diagnosis for Alzheimer
This repository hosts a Computer-Aided Diagnosis for Alzheimer early phases using *magnetic resonance imaging* (MRI) and *convolutional neural networks* (CNN). 

## About the dataset
The dataset was taken from [Kaggle](https://www.kaggle.com/code/aashidutt3/alzheimer-classification-with-mri-images/input) and contains MRI images from Alzheimer's early stages; in the dataset an original and an augmented version can be found. Augmented dataset was used for training, validation and testing.

The dataset is divided into four categories as shown:

| Category           | Augmented_Dataset  | Original_Dataset   |
|--------------------|--------------------|--------------------|
| Non_demented       | 9600 images        | 3200 images        |
| VeryMild_demented  | 8960 images        | 2240 images        |
| Mild_demented      | 8960 images        | 896 images         |
| Moderate_demented  | 6464 images        | 64 images          |

## About the model

### Architecture
The main model consists of a CNN with the following architecture

***First Block*** (Spatial Dropout 0.2)
1. Convolutional 32 neurons (3 x 3 kernel), RELU
2. Batch Normalization
3. Convolutional 32 neurons (3 x 3 kernel), RELU
4. Batch Normalization
5. Max Pooling (2 x 2 kernel)

***Second Block*** (Spatial Dropout 0.3)
1. Convolutional 64 neurons (3 x 3 kernel), RELU
2. Batch Normalization
3. Convolutional 64 neurons (3 x 3 kernel), RELU
4. Batch Normalization
5. Max Pooling (2 x 2 kernel)

***Third Block*** (Spatial Dropout 0.4)
1. Convolutional 128 neurons (3 x 3 kernel), RELU
2. Batch Normalization
3. Convolutional 128 neurons (3 x 3 kernel), RELU
4. Batch Normalization
5. Max Pooling (2 x 2 kernel)

***Output/Classification Block*** (Dropout 0.5)
1. Flatten
2. Dense Layer 256 neurons, RELU
3. Batch Normalization
4. Dense Output Layer 4 neurons, SOFTMAX

### Training & Validation

### Testing & Results

## Prerequisites and Dependencies
Make sure you have the following installed:
- Python 3.x (We are using 3.10)

This project uses the following Python libraries:
- numpy
- pandas
- seaborn
- matpolib
- kagglehub
- tensorflow
- scikit-learn

## Usage


## Contributors
🔹 [Ingrid](https://github.com/ingridperezs)
🔹 [Juan](https://github.com/juanuwo)
