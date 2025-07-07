🌱 Plant Seedlings Classification using Deep Learning

🧠 Project Overview
This project utilizes computer vision and Deep Learning to automate the classification of plant seedlings into 12 distinct species using a Convolutional Neural Network (CNN) model. By leveraging image data, preprocessing techniques, and neural network architectures, this model aims to reduce manual labor in agriculture, improving efficiency and accuracy in plant identification.

📌 Problem Statement
Despite advances in agri-tech, manual identification of plant species remains labor-intensive. This project proposes a CNN-based solution to classify seedlings, aiming to: automatically

1. Reduce human effort in identifying plants
2. Increase classification accuracy
3. Enable scalable and sustainable crop monitoring solutions

🎯 Objectives
1. Build an end-to-end pipeline to classify images of plant seedlings
2. Perform Exploratory Data Analysis (EDA)
3. Implement preprocessing steps like resizing, denoising, and normalization
4. Train, validate, and evaluate a CNN model

📊 Dataset
Source: Aarhus University Signal Processing Group
Classes: 12 species

Format:
images.npy: Image data (4750 images)
Labels.csv: Corresponding species labels


🌿 Plant Species
mathematica
Black-grass, Charlock, Cleavers, Common Chickweed, Common Wheat,
Fat Hen, Loose Silky-bent, Maize, Scentless Mayweed, 
Shepherds Purse, Small-flowered Cranesbill, Sugar beet


🧪 Methodology
1. Data Loading & Preprocessing
Images converted from BGR to RGB
Resized from 128×128 to 64×64 pixels
Gaussian blur applied for denoising
Normalized pixel values
One-hot encoded labels

2. EDA Highlights
Visualized class imbalance
Random sample plotting for each species

3. Model Architecture
A basic CNN (model_0) with:
2 convolutional layers (ReLU, He initialization)
2 max-pooling layers
2 dense layers (Dropout for regularization)
Softmax output for 12 classes

📈 Evaluation
Dataset Split:
Training: 70%
Validation: 15%
Testing: 15%

Metrics:
Accuracy
Confusion Matrix

Visualization:
Training curves
Misclassified examples

📂 Project Structure
CV_Project_Full_Code_Notebook.ipynb
├── images.npy
├── Labels.csv
├── Model architecture
├── Data preprocessing
└── Evaluation & metrics

💡 Future Scope
1. Implement transfer learning using pre-trained models like ResNet or EfficientNet
2. Apply class balancing techniques (SMOTE, augmentation)
3. Deploy as a web app using Flask or Streamlit
4. Extend to real-time camera-based seedling detection
