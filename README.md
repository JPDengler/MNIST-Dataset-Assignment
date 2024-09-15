# MNIST Handwritten Digit Classification using Keras

## Project Overview

This project demonstrates the use of a neural network to classify handwritten digits from the MNIST dataset. It was developed as part of the CS 370 course assignment, where various parameters of the neural network were modified to observe their impact on accuracy. 

The experiments include adjusting the number of **epochs**, **batch size**, and **hidden neurons** to find the optimal configuration for training, validation, and test accuracy.

## Files

- **Dengler_Joseph_Assignment1.ipynb**: The Jupyter Notebook containing the code, markdown explanations, and experiment results.
- **README.md**: This file, providing an overview of the project.
- **Results**: Output and logs are included in the notebook.

## Dataset

The project uses the **MNIST handwritten digits dataset**, which is automatically loaded through the `Keras` library. The dataset consists of 60,000 training samples and 10,000 test samples of 28x28 pixel grayscale images of handwritten digits (0-9).

## Experiments

### 1. Modifying Epochs:
- Epochs: 10, 20, 30
- Observations: Increasing the number of epochs led to improved accuracy, with diminishing returns after 20 epochs. Best results were achieved with 30 epochs.

### 2. Modifying Batch Size:
- Batch sizes: 64, 128 (default), 256
- Observations: A smaller batch size of 64 resulted in the highest accuracy, while larger batch sizes led to reduced performance.

### 3. Modifying Hidden Neurons:
- Hidden neurons: 64, 128 (default), 256
- Observations: Increasing the number of hidden neurons to 256 resulted in the highest test accuracy, though it required longer training times.

## Installation & Requirements

1. **Keras**: Install Keras for deep learning.
    ```
    pip install keras
    ```
2. **TensorFlow**: Backend for Keras.
    ```
    pip install tensorflow
    ```
3. **Jupyter Notebook**: The project is developed in Jupyter Notebook.
    ```
    pip install notebook
    ```

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/mnist-keras-classification.git
    cd mnist-keras-classification
    ```
2. Launch Jupyter Notebook:
    ```bash
    jupyter notebook Dengler_Joseph_Assignment1.ipynb
    ```

3. Run the cells in the notebook to see the model training, validation, and test results.

## Results Summary

The best model configuration:
- **Epochs**: 30
- **Batch Size**: 64
- **Hidden Neurons**: 256
- **Test Accuracy**: 96.97%

## Author

Joseph Dengler

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
