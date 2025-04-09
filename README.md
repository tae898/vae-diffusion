# VAE and Diffusion Models: A Step-by-Step Guide

This repository contains educational Jupyter notebooks that explore the theory and
implementation of generative models, specifically **Variational Autoencoders (VAEs)**
and **Diffusion Models**. These notebooks are designed to provide a clear, step-by-step
understanding of how these powerful generative AI techniques work.

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
- Implementation of a VAE with both Bernoulli and Gaussian likelihoods
- Comparison of different likelihood models and their effects on image generation
  quality

---

### [`02.vae-without-encoder.ipynb`](./02.vae-without-encoder.ipynb) – Simplified VAE (Decoder-Only)

This notebook explores a "VAE-like" model that omits the encoder:

- One-step fixed corruption process as "inference"
- Connection between this simplified model and diffusion models
- Implementation of a noise prediction objective
- Demonstration of how this approach performs on MNIST data

---

### [`03.diffusion.ipynb`](./03.diffusion.ipynb) – Diffusion Models

This comprehensive notebook dives into diffusion models:

- Forward and reverse processes in diffusion models
- Beta schedules (linear vs. cosine)
- Variational inference and the ELBO objective for diffusion
- Simplified noise prediction objective
- Implementation of a diffusion model with:
  - ShuffleNet-based UNet architecture
  - Exponential Moving Average (EMA) for stable training
  - Time embedding and conditioning
  - Cosine beta schedule

---

## Contributing

Contributions are what make the open source community such an amazing place to be learn,
inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
1. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
1. Run `make test && make style && make quality` in the root repo directory, to ensure
   code quality.
1. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
1. Push to the Branch (`git push origin feature/AmazingFeature`)
1. Open a Pull Request

---

## Authors

- [Taewoon Kim](https://taewoon.kim/)
