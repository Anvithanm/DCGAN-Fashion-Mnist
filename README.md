# 🧵 Fashion-MNIST Image Generation using DCGAN

This project uses a **Deep Convolutional Generative Adversarial Network (DCGAN)** built with TensorFlow to generate fashion images similar to those in the Fashion-MNIST dataset. It showcases how adversarial training between a generator and discriminator can create realistic-looking clothing images.

## 📁 Dataset

- **Fashion-MNIST**: A dataset of 28x28 grayscale images of clothing items such as shirts, sneakers, bags, and more.
- Provided by Zalando and available via TensorFlow/Keras datasets module.

## 🧠 Model Architecture

### Generator
- Takes in random noise (latent vector).
- Transposed convolution layers are used to upsample the input.
- Outputs a 28x28 grayscale image resembling a fashion item.

### Discriminator
- Takes in an image (either real or generated).
- Convolutional layers are used to downsample and extract features.
- Outputs a single value (0–1) indicating the probability that the input image is real.

## 🔁 Training Process

- The generator attempts to produce fake images that resemble the real ones.
- The discriminator learns to distinguish between real and fake images.
- Both networks are trained in an adversarial loop:
  - The **generator** gets better at fooling the discriminator.
  - The **discriminator** improves at spotting fake images.

## 🎯 Objective

Generate realistic fashion images after adversarial training.

## ✅ Results

After training:
- The generator model was used to produce **three distinct clothing images**.
- These images demonstrate how the network learns to generate convincing clothing patterns.

Example outputs (generated images) are available in the `outputs/` folder.

## 📦 Dependencies

- Python 3.x
- TensorFlow
- NumPy
