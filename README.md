# Face Mask Detection using NN/CNN 😷

![Face Mask Detection](https://img.shields.io/badge/Python-3.8%2B-blue) ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange) ![OpenCV](https://img.shields.io/badge/OpenCV-4.5.3-green) ![License](https://img.shields.io/badge/License-MIT-green)

## 📖 Overview

This project is a Face Mask Detection system using Convolutional Neural Networks (CNNs). It classifies images as either "with mask" or "without mask," leveraging real-time video feeds. The system was built using **Python**, **TensorFlow/Keras**, and **OpenCV**, and it was trained on a dataset from Kaggle. This tool is particularly relevant for ensuring public safety during the COVID-19 pandemic.

## 🎯 Features

- **Real-time Detection**: Identify mask compliance in live video feeds.
- **High Accuracy**: Achieved with CNN architectures.
- **Easy to Use**: Can be run on Google Colab or Jupyter Notebook.

## 📂 Dataset

The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/omkargurav/face-mask-dataset). It includes images of people with and without face masks.

### Downloading the Dataset

**Option 1: Using Kaggle API**

```bash
# Configure the path to the kaggle.json file
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

# Fetch the dataset from Kaggle
!kaggle datasets download -d omkargurav/face-mask-dataset

# Extract the compressed dataset
from zipfile import ZipFile
dataset = '/content/face-mask-dataset.zip'

with ZipFile(dataset, 'r') as zip:
    zip.extractall()
    print("The Dataset is extracted!")


## ⚙️ Installation

---

## Requirements

- Python 3.8+
- TensorFlow 2.0+
- OpenCV 4.5.3
- NumPy
- Matplotlib

To install the required packages, run the following command:

```bash
pip install tensorflow opencv-python numpy matplotlib
