Indian Sign Language Classification using MobileNetV2 and ResNet152V2

This project focuses on classifying Indian Sign Language (ISL) hand gestures using two deep learning architectures: MobileNetV2 and ResNet152V2.
The goal is to compare their performance in terms of accuracy, model complexity, and suitability for real-time applications.

The dataset used is already cleaned, filtered, and ready for training, requiring no preprocessing apart from resizing and normalization inside the models.

📁 Project Structure
project/
│
├── data/          # Ready-to-use dataset (train/test folders or classes)
├── src/           # Training scripts, model definitions, evaluation code
├── results/       # Model weights, accuracy/loss graphs, confusion matrices
├── requirements/  # Python dependencies (requirements.txt)
└── README.md

🎯 Objective

To determine which model — MobileNetV2 or ResNet152V2 — performs better for ISL image classification, considering:

Accuracy

Training time

Inference speed

Model size

Practical deployment feasibility

🚀 Features

Uses pre-filtered and ready-to-train Indian Sign Language datasets

Transfer-learning implementation of MobileNetV2 & ResNet152V2

Automatic dataset splitting (if needed) within training scripts

Graphical comparison of model performance

Saved weights, evaluation metrics, and confusion matrices

Organized code and results for reproducibility

🛠 Installation

Clone the repository:

    git clone https://github.com/HaaKaaL/Comparison-of-CNN-Models.git
    cd Comparison-of-CNN-Models


Install dependencies:

    pip install -r requirements/requirements.txt


Recommended Python version: 3.8+

▶️ Usage
1. Ensure your dataset is placed inside data/

Folder structure may look like:

data/
 ├── A/
 ├── B/
 ├── C/
 └── ...

2. Train the MobileNetV2 Model

       python src/train_mobilenetv2.py

3. Train the ResNet152V2 Model

       python src/train_resnet152v2.py

4. Evaluate & Compare Models

       python src/evaluate_models.py


Results (graphs, logs, saved models) will appear in the results/ directory.

📊 Results & Comparison

This project generates and stores the following inside the results/ folder:

Training/Validation accuracy curves

Training/Validation loss curves

Confusion matrices for both models

Summary comparison of performance metrics

Saved model weights (.h5 or .keras format)

Example comparison format:

Metric	MobileNetV2	ResNet152V2
Accuracy	X%	Y%
Training Time	Fast	Slower
Model Size	Lightweight	Heavy
Inference Speed	High	Moderate

(Replace X and Y with your actual metrics.)



📦 Technologies Used

Python

TensorFlow / Keras

NumPy, Pandas

Scikit-learn

Matplotlib / Seaborn
