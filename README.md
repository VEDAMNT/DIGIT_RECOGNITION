# DIGIT_RECOGNITION
# MNIST Digit Classification

This project involves training a simple neural network to classify handwritten digits from the MNIST dataset using TensorFlow and Keras. The dataset is split into training and testing sets, with preprocessing steps applied to prepare the data for model training.

## Dependencies

- Python 3.x
- numpy
- pandas
- matplotlib
- tensorflow

You can install the required packages using pip:

```bash
pip install numpy pandas matplotlib tensorflow
```
Dataset
The project uses the MNIST dataset, which should be in CSV format:

train.csv: Training data including pixel values and labels.
test.csv: Testing data including pixel values and labels.
The dataset files should be placed in the root directory of the project.

## Code Explanation

Data Loading:
The dataset is loaded from CSV files using pandas.
Training features (X_train) and labels (y_train) are separated.
Testing features (X_test) are also extracted.

Data Preprocessing:
Pixel values are normalized to the range [0, 1].
Data is reshaped to add a channel dimension.
Labels are one-hot encoded for training and evaluation.

Model Definition:
A Sequential model with three dense layers is created.
The first layer flattens the input data, followed by two hidden layers with ReLU activation.
The output layer uses the softmax activation function to predict digit classes.

Model Training:
The model is compiled with the Adam optimizer and categorical crossentropy loss function.
Training is performed with a validation split of 10%.

Model Evaluation:
The model is evaluated on the test set.
Accuracy is printed to the console.

Prediction:
An example prediction is made for the first image in the test set.
The predicted digit is printed to the console.

Visualization:
The example image is reshaped and displayed using matplotlib.

Usage
Ensure that train.csv and test.csv are in the project directory.
Run the script:
```bash
python script_name.py```
Replace script_name.py with the name of your Python file.
