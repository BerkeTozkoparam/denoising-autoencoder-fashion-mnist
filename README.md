# Denoising Autoencoder with Latent Space Visualization

This repository contains an implementation of a Stacked Denoising Autoencoder using TensorFlow and Keras. The project utilizes the Fashion MNIST dataset to demonstrate image restoration techniques and unsupervised feature learning.

The primary objective is to train a neural network to reconstruct original images from inputs corrupted with Gaussian noise. Additionally, the project visualizes the compressed latent space using t-SNE to analyze how the model clusters different clothing categories without explicit supervision.

## Project Overview

Autoencoders are a type of artificial neural network used to learn efficient data codings in an unsupervised manner. This project extends the basic autoencoder architecture to a "Denoising Autoencoder," which is trained to ignore "noise" in the input data.

Key components of this project include:
1.  **Noise Injection:** Artificially adding Gaussian noise to the dataset to simulate data corruption.
2.  **Architecture:** A stacked dense network that compresses the 784-dimensional input into a 16-dimensional bottleneck layer.
3.  **Visualization:** Using t-SNE (t-Distributed Stochastic Neighbor Embedding) to project the high-dimensional latent space into 2D for analysis.
4.  **Evaluation:** Measuring reconstruction quality using the Structural Similarity Index (SSIM) and Loss curves.
<img width="803" height="643" alt="Ekran Resmi 2025-12-11 00 14 35" src="https://github.com/user-attachments/assets/f5a450d3-e06b-4a97-8ab5-5085060ada06" />
<img width="855" height="458" alt="Ekran Resmi 2025-12-11 00 13 36" src="https://github.com/user-attachments/assets/8ff7e323-cad9-4cad-bf61-809b21e53741" />

## Dependencies

To run this project, you need the following Python libraries:

* numpy
* matplotlib
* seaborn
* scikit-learn
* tensorflow
* scikit-image

You can install the dependencies using pip:

```bash
pip install numpy matplotlib seaborn scikit-learn tensorflow scikit-image
