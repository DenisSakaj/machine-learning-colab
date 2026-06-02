Fashion-MNIST Image Classification & Explainability
A machine learning project built in Python (Google Colab) that trains and compares multiple classification models on the Fashion-MNIST dataset, then applies explainability techniques to interpret model decisions.
Overview
This project explores the full ML pipeline — from data preprocessing and model training to performance evaluation and visual explainability. Three model architectures are implemented and compared, with Grad-CAM and LIME used to make model predictions interpretable.
Models Implemented

Convolutional Neural Network (CNN) — deep learning model leveraging spatial feature extraction
Artificial Neural Network (ANN) — fully connected feedforward network
Logistic Regression — classical baseline classifier for comparison

Explainability Techniques

Grad-CAM (Gradient-weighted Class Activation Mapping) — highlights which regions of an image most influenced the model's prediction
LIME (Local Interpretable Model-Agnostic Explanations) — generates locally faithful explanations for individual predictions

Dataset
Fashion-MNIST — 70,000 grayscale images (28×28px) across 10 clothing categories:
LabelClass0T-shirt/top1Trouser2Pullover3Dress4Coat5Sandal6Shirt7Sneaker8Bag9Ankle boot

60,000 training images
10,000 test images

Evaluation Metrics
Each model is evaluated using:

Accuracy
Precision
Recall
Confusion Matrix

Tech Stack

Python
TensorFlow / Keras
Scikit-learn
NumPy
Pandas
Matplotlib
Google Colab

How to Run

Open the notebook in Google Colab:

Go to colab.research.google.com
Click File → Open notebook → GitHub
Paste this repo URL


Run all cells in order (Runtime → Run all)


No local setup required — all dependencies are available in Colab by default.

Project Structure
machine-learning-colab/
├── CN6005_Grad_CAM,_LIME,_Confusion_Matrixes.ipynb   # Main notebook
└── README.md
Key Findings

CNN achieved the strongest classification performance across all 10 categories, benefiting from convolutional feature extraction
Grad-CAM visualisations confirmed models focused on relevant garment regions rather than background noise
LIME provided per-prediction explanations, highlighting which pixel regions drove individual classifications
Logistic Regression served as a useful baseline, showing the performance gap between classical and deep learning approaches

Future Improvements

Hyperparameter tuning for CNN (learning rate, dropout, batch size)
Data augmentation to improve generalisation
Deploy best model via a Flask or FastAPI endpoint
Add interactive prediction demo

License
MIT
