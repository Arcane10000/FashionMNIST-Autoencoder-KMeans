Fashion-MNIST Clustering using Autoencoder + KMeans (CSE425)

Overview
This project was developed as part of CSE425 – Neural Networks.
It applies unsupervised learning techniques on the Fashion-MNIST dataset by training an Autoencoder to learn compressed latent representations of images, followed by KMeans clustering on the encoded features to group similar fashion items.

Dataset
- Fashion-MNIST (28x28 grayscale images, 10 classes)
- Loaded via Hugging Face Datasets
- Images are normalized to [0,1] and flattened for the model

Method
1. Train an Autoencoder to learn a latent feature space
2. Apply KMeans clustering (k=10) on the latent vectors
3. Visualize clusters using t-SNE
4. Evaluate using Purity, Silhouette, ARI, and NMI (labels used only for evaluation)

Results (from report)
- Purity: 0.5541
- Silhouette: 0.2091
- ARI: 0.3444
- NMI: 0.5217

How to Run
1. Open the notebook:
   notebooks/CSE425_project_final.ipynb
2. Install dependencies if needed:
   pip install numpy pandas matplotlib scikit-learn torch torchvision datasets

Notes
- Ground-truth labels were used only for evaluation
- This project focuses on representation learning and clustering, not classification

Author
Fardeen Rahman
CSE425 – Neural Networks
BRAC University
