# VAE and Diffusion Models: A Step-by-Step Guide

[![DOI](https://zenodo.org/badge/962009233.svg)](https://doi.org/10.5281/zenodo.15574231)

This repository contains educational Jupyter notebooks that explore the theory and
implementation of generative models, specifically **Variational Autoencoders (VAEs)**
and **Diffusion Models**. These notebooks are designed to provide a clear, step-by-step
understanding of how these powerful generative AI techniques work.

---

## 🚀 Installation

To run the notebooks in this repository, you'll need Python 3.8+ and the following dependencies:

```bash
pip install -r requirements.txt
```

The main dependencies are:
- PyTorch (for deep learning models)
- torchvision (for computer vision utilities)
- matplotlib (for visualization)
- tqdm (for progress bars)

---

## 📚 What You'll Learn

- The mathematical foundations behind VAEs and diffusion models
- How to implement these models from scratch using PyTorch
- The connection between VAEs and diffusion models
- How to generate MNIST digits using these techniques

---

## 🗂️ Notebook Overview

### [`01.vae.ipynb`](./01.vae.ipynb) – Variational Autoencoders

This notebook covers the fundamental concepts of Variational Autoencoders (VAEs):

- Motivation behind generative models and latent variable models
- The Evidence Lower Bound (ELBO) objective
- Reparameterization trick for training VAEs
- Implementation of VAEs using both Multi-Layer Perceptron (MLP) and Convolutional
  Neural Network (CNN) architectures
- Exploration of both Bernoulli and Gaussian likelihoods for the decoder
- Comparison of different likelihood models and architectures, and their effects on
  image generation quality for MNIST digits

---

### [`02.vae-without-encoder.ipynb`](./02.vae-without-encoder.ipynb) – Simplified VAE (Decoder-Only)

This notebook explores a "VAE-like" model that omits the encoder:

- One-step fixed corruption process as "inference"
- Connection between this simplified model and diffusion models
- Implementation of a noise prediction objective
- Demonstration of how this approach performs on MNIST data
- Compare the classical CNN architecture with the U-Net CNN architecture

---

### [`03.diffusion.ipynb`](./03.diffusion.ipynb) – Diffusion Models

This comprehensive notebook dives into diffusion models:

- Forward and reverse processes in diffusion models
- Beta schedules (linear)
- Variational inference and the ELBO objective for diffusion
- Simplified noise prediction objective
- Implementation of a diffusion model with:
  - UNet architecture
  - Time embedding and conditioning
  - Linear beta schedule

### Next

- Conditional generation, e.g., class, text, with VAE and diffusion.
- VAE and diffusion working together, e.g., VAE as an encoder diffusion as a decoder.
- Discrete modality, e.g., table, graph, text, etc, with non Gaussian and continuous
  distributions, e.g., discrete categorical.

