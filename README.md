# Variational Autoencoder GAN for Faces

A PyTorch project combining a **Variational Autoencoder (VAE)** and **GAN** to generate realistic human faces.  
This hybrid approach leverages the reconstruction ability of VAEs and the adversarial training of GANs.

## Features
- Hybrid VAE-GAN architecture
- Realistic face generation
- Latent space exploration for image variations
- Easy experimentation with network architectures and hyperparameters

## Variational Autoencoder Math
- Encoder outputs mean `μ` and variance `σ²` for the latent space
- Latent vector `z` is sampled as: `z = μ + σ * ε,  ε ~ N(0,1)`
- Loss combines reconstruction loss and KL divergence: `L = E_q(z|x)[log p(x|z)] - KL(q(z|x) || p(z))`

## Research Papers
- Kingma, D.P. & Welling, M. (2013). [Auto-Encoding Variational Bayes](https://arxiv.org/abs/1312.6114)  
- Goodfellow, I. et al. (2014). [Generative Adversarial Nets](https://arxiv.org/abs/1406.2661)  
- Larsen, A. B. L. et al. (2015). [Autoencoding beyond pixels](https://arxiv.org/abs/1512.09300)

## Usage
1. Clone the repo:  
   `git clone https://github.com/demss233/variational-autoencoder-gan-faces.git`  
   `cd variational-autoencoder-gan-faces`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook: `jupyter notebook variational-autoencoder-with-pytorch.ipynb`
