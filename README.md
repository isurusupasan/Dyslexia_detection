# Dyslexia_detection
Identification of Dyslexia  in Children Utilizing the Gamified Learning Environments

Overview:
-----------
This project uses a Convolutional Neural Network (CNN) to classify images into two categories:
- Dyslexic
- Non-Dyslexic

The model has been trained using labeled image data stored in the following directories:
- images2/dyslexic/
- images2/non_dyslexic/

  Requirements:
---------------
Install the required Python packages using:

pip install tensorflow,keras,pillow scikit-learn,matplotlib,opencv-python

Model details:
--------------------
Model I.ipynb           # Main Jupyter Notebook with model training and evaluation
images2/
  ├── dyslexic/         # Images labeled as dyslexic
  └── non_dyslexic/     # Images labeled as non-dyslexic

Model Architecture:
---------------------
- Input Layer: 64x64 RGB image
- Hidden Layers: Convolutional, MaxPooling, Flatten, Dense layers (detailed in notebook)
- Output Layer: Binary classification (0: Dyslexic, 1: Non-Dyslexic)
- Loss Function: binary_crossentropy
- Optimizer: Adam
- Metrics: accuracy

How to Run:
---------------
1. Place your dataset inside images2/ with subdirectories dyslexic/ and non_dyslexic/.
2. Open and run all cells in Model I.ipynb.
3. The model will train and provide evaluation metrics on the test set.

Output
---------
- Training accuracy and loss graphs
- Confusion matrix
- Classification report

Notes
--------
- Random seed is set to ensure reproducibility.
- Dataset is shuffled and split into training and test sets.
- Make sure image formats are .jpg
