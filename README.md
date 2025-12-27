# Fashion-MNIST Clustering using Autoencoder + KMeans (CSE425)

## Overview
This is my CSE425 (Neural Network) project which applies unsupervised learning on the Fashion-MNIST dataset. An Autoencoder is trained to learn compressed latent representations of images, and KMeans clustering is applied on the encoded features to group similar fashion items.

## Dataset
- Fashion-MNIST (28×28 grayscale images, 10 classes)
- Loaded via Hugging Face Datasets
- Images are normalized to [0,1] and flattened for the model

## Method
1. Train an Autoencoder to learn a latent feature space
2. Apply KMeans clustering (k=10) on the latent vectors
3. Visualize clusters using t-SNE
4. Evaluate using Purity, Silhouette, ARI, and NMI (labels used only for evaluation)

## Results (from report)
- Purity: 0.5541
- Silhouette: 0.2091
- ARI: 0.3444
- NMI: 0.5217

## How to run
Open the notebook:
- notebooks/CSE425_project_final.ipynb

Install dependencies (optional):
```bash
pip install -r requirements.txt
