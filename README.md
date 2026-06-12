\# Pneumonia Detection Using Deep Learning



\## Overview

This project uses deep learning to classify chest X-ray images into two categories: \*\*Normal\*\* and \*\*Pneumonia\*\*.  

The main goal is to compare different deep learning models and identify the best model for pneumonia detection from X-ray images.



## Dataset

The project uses the **Chest X-Ray Images (Pneumonia)** dataset from Kaggle.

Dataset link:
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

The dataset contains two classes:

* NORMAL
* PNEUMONIA

Dataset structure:

* Train: 5216 images
* Validation: 16 images
* Test: 624 images

**Note:**
The dataset is not included in this repository due to its large size.
This repository is intended to showcase the notebook, methodology, model comparison, and saved results.



\## Models Used

Three deep learning models were used and compared:



1\. Custom CNN Model

2\. VGG16 Transfer Learning

3\. Improved VGG16 with Data Augmentation and Class Weights




\## Methodology

The X-ray images were resized and normalized before training.  

A custom CNN model was used as the baseline model.  

Then, VGG16 was applied using transfer learning.  

Finally, the VGG16 model was improved by using data augmentation and class weights to improve the performance.




\## Results

The best model was the \*\*Improved VGG16\*\* model.



| Model | Test Accuracy |

|---|---:|

| Custom CNN | 73.24% |

| VGG16 | 71.79% |

| Improved VGG16 | 87.82% |




\## Best Model Performance



| Class | Precision | Recall | F1-score |

|---|---:|---:|---:|

| NORMAL | 0.99 | 0.68 | 0.81 |

| PNEUMONIA | 0.84 | 0.99 | 0.91 |



Overall Accuracy: \*\*88%\*\*




\## Tools and Libraries

\- Python

\- TensorFlow / Keras

\- NumPy

\- Matplotlib

\- Seaborn

\- Scikit-learn

\- Jupyter Notebook




\## Project Files

\- `Pneumonia\_Detection\_Using\_Deep\_Learning.ipynb`  

&#x20; Main notebook that contains data preprocessing, model training, evaluation, and prediction.



\- `README.md`  

&#x20; Project description and documentation.



\- `requirements.txt`  

&#x20; Required Python libraries to run the project.




\## How to Run

1\. Download the dataset.

2\. Place the dataset folder inside the project directory.

3\. Install the required libraries:



```bash

pip install -r requirements.txt  





jupyter notebook Pneumonia\_Detection\_Using\_Deep\_Learning.ipynb



Run the notebook cells step by step





Conclusion



The Improved VGG16 model achieved the best performance with a test accuracy of 87.82%.

The model showed strong ability to detect pneumonia cases, especially with a high recall for the Pneumonia class.

