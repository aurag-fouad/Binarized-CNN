# CIFAR-10 Classification with CNN and Binarized CNN

This project demonstrates a comparison between a standard Convolutional Neural Network (CNN) and a Binarized Neural Network (BNN) proposed by [Hubara, et al. (2018)](https://www.jmlr.org/papers/volume18/16-456/16-456.pdf) for image classification on the CIFAR-10 dataset. The CNN was implemented using PyTorch, achieving 72.95% accuracy, while the binarized CNN was adapted from the binarization method proposed by Hubara et al. (2018) and achieved 62.35% accuracy using binary weights and activations.

## Project Overview

The notebook in this repository covers the following:
1. **CNN Implementation**: A standard CNN model is trained and evaluated on CIFAR-10, reaching an accuracy of 72.95%.
2. **Binarized CNN**: Using the binarization technique by Hubara et al., we implemented a BNN, which uses binary weights and activations to reduce computational cost. The binarized CNN achieved 62.35% accuracy on CIFAR-10.
3. **Comparison of Configurations**: We tested both models with different configurations, combining cross-entropy and hinge losses with SGD and Adam optimizers.

## Experimental Results

The following graph illustrates the accuracy results of various configurations for the CNN and binarized CNN models.

![Accuracy Comparison](https://github.com/aurag-fouad/Binarized-CNN/blob/main/acc%20comparison.png)

- **Standard CNN**: Achieved the highest accuracy (72.95%) with Cross-Entropy loss and Adam optimizer.
- **Binary CNN (B_CNN)**: Achieved a maximum accuracy of 62.35% with Cross-Entropy loss and Adam optimizer, showing a 10.6% difference compared to the standard CNN.

## Installation

To run this project, clone this repository and install the required dependencies:

```bash
git clone https://github.com/aurag-fouad/Binarized-CNN.git
cd Binarized-CNN
```

Ensure you have the following in your requirements.txt:
- torch
- torchvision
- numpy
- matplotlib

## Usage

You can open the Jupyter notebook, and re-run the cells to train both CNN and Binarized CNN models on CIFAR-10 and observe the results.

1. Run the CNN Model: Train and evaluate the standard CNN on CIFAR-10.
2. Run the Binarized CNN Model: Train and evaluate the binarized CNN using binary weights and activations.
3. Experiment with Configurations: Adjust the loss functions (Cross-Entropy, Hinge) and optimizers (SGD, Adam) as needed.

# Reference
- Hubara, Itay, et al. "Quantized neural networks: Training neural networks with low precision weights and activations." Journal of Machine Learning Research 18.187 (2018): 1-30.

