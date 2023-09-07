# Neural Network for Digit Recognition
This repository contains Python code for training and using a neural network to recognize handwritten digits. The code utilizes the popular Python libraries NumPy and Pandas for data manipulation and the Matplotlib library for visualization.
## Overview
The code in this repository accomplishes the following tasks:
### Data Loading and Preprocessing:
The code starts by loading training data from a CSV file (e.g., train.csv). This data typically contains images of handwritten digits (0-9) and their corresponding labels. The dataset is shuffled, split into a development set and a training set, and the pixel values of the images are normalized to the range [0, 1].
### Neural Network Architecture:
The neural network used in this code has three hidden layers with ReLU activation functions and a softmax output layer. The architecture is as follows:
- Input layer: 784 units (corresponding to a 28x28 pixel image)
- Hidden layer 1: 200 units
- Hidden layer 2: 200 units
- Hidden layer 3: 10 units (for classifying digits 0-9)
- Output layer: 10 units (corresponding to the possible digit classes)
### Training the Neural Network:
The neural network is trained using gradient descent with backpropagation. The code initializes the network's weights and biases, performs forward and backward propagation, and updates the parameters iteratively. During training, it prints out the accuracy of predictions on the training data at regular intervals.
### Making Predictions:
After training, the network can make predictions on new data. You can use the make_predictions function to predict the digit in an image.
### Visualization:
The code includes functionality to visualize a specific image from the training dataset and predict the digit in that image.
## Usage
1. Ensure you have Python installed, along with the required libraries: NumPy, Pandas, and Matplotlib.
2. Clone this repository to your local machine.
3. Provide your own training data by replacing the path to the CSV file in the data = pd.read_csv(...) line.
4. Customize the neural network architecture, training parameters, and visualization as needed for your specific application.
5. Run the code in a Python environment. Training will print the progress and accuracy on the training data, and you can use the test_prediction function to visualize and predict digits from the training dataset.



Feel free to modify this README to include additional information or specific instructions as needed for your project.
