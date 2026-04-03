# Handwritten Digit Generation with DCGAN

This repository implements a **Deep Convolutional Generative Adversarial Network (DCGAN)** in PyTorch to generate handwritten digits similar to those in the MNIST dataset.

## Architecture

The project consists of two competing networks: 1. **The Generator:** Learns to create realistic images from a noise vector using `ConvTranspose2d` layers. 2. **The Discriminator:** A convolutional binary classifier that learns to distinguish between real MNIST images and "fake" images produced by the generator.

## Training Details

-   **Dataset:** MNIST (Handwritten Digits).
-   **Optimizer:** Adam ($\beta_1=0.5, \beta_2=0.999$).
-   **Loss:** Binary Cross Entropy with Logits (`BCEWithLogitsLoss`).
-   **Weight Initialization:** Custom normal distribution initialization for convolutional and batch-norm layers.

## Result

As training progresses through the epochs, the generator evolves from producing random noise to clear, recognizable digits.

