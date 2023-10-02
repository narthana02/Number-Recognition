# Number-Recognition
Here's a summary of the provided code and the key inferences drawn from it:

1. **Data Loading and Preprocessing:**
   - The code starts by importing necessary libraries, including NumPy, Matplotlib, and Keras.
   - It loads the MNIST dataset, which contains handwritten digit images and their corresponding labels.
   - The images are reshaped to a format suitable for training a neural network and are normalized to the range [0, 1].
   - The labels are one-hot encoded to represent the digit classes.

2. **Exploratory Data Analysis (EDA):**
   - The code performs EDA by visualizing the distribution of digit labels in the training set using a histogram.
   - It also displays sample images from the training set along with their corresponding labels, allowing you to visually inspect the data.

3. **Neural Network Model:**
   - A neural network model is defined using Keras. It consists of a flattening layer, followed by two dense (fully connected) hidden layers with ReLU activation functions, and an output layer with softmax activation for classification.

4. **Model Compilation and Training:**
   - The model is compiled with the Adam optimizer and categorical cross-entropy loss.
   - It is trained on the training data for 10 epochs with a batch size of 128, using 20% of the data as a validation set.

5. **Training and Validation Plots:**
   - The code generates two sets of plots:
     - Training and validation loss over epochs.
     - Training and validation accuracy over epochs.
   - These plots provide insights into the model's training performance.

6. **Model Evaluation:**
   - The trained model is evaluated on the test data, and the test accuracy is displayed.

7. **Digit Recognition Example:**
   - The code includes a `recognize_digit` function that takes an image and predicts the digit it represents.
   - An example digit recognition is performed on a sample image from the test set, showing the predicted and actual digits.

Inferences:
- The model achieves a test accuracy of around 97% after training for 10 epochs.
- The EDA plots provide an overview of the dataset's label distribution and sample images.
- The training and validation loss curves indicate that the model converges during training without significant overfitting.
- The training and validation accuracy curves show that the model's accuracy increases with training epochs.

Overall, this code demonstrates how to build, train, and evaluate a neural network model for handwritten digit recognition using the MNIST dataset. It also includes EDA and visualization techniques to understand the data and training progress.
