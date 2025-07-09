# Traffic Sign Classification Using Classical and CNN Models (2025 Project)

## Overview  
This project classifies German traffic signs into 43 classes using both manual feature extraction methods (HOG, color histograms, LBP, contours) and a LeNet-5 convolutional neural network. It includes feature engineering, model training, evaluation, and comparison.

## Directory Structure  
- `train/`: Contains training images  
  - `train_metadata.csv`: Metadata file with image IDs, filenames, and class labels  
- `test/`: Contains test images  
  - `test_metadata.csv`: Metadata with image IDs and filenames (no labels)  
- `traffic-sign-classification.ipynb`: Jupyter notebook containing all code for preprocessing, training, and evaluation  
- `cnn_eval_state.pt`: Saved CNN model weights for evaluation reproducibility  
- `cnn_kaggle_state.pt`: Saved CNN model weights for Kaggle test submission reproducibility  
- `gtsrb-classification.pdf`: Technical report on the project methodology and results  
- `README.md`: This file  

## Data  
- 5488 training images with class labels  
- 2353 test images without labels  
- 43 total traffic sign classes  
> *Note: Training and test images are not included and must be downloaded from [GTSRB official site](link-to-dataset)*  

## Execution Instructions  
1. Python version: 3.12.7  
2. Install required libraries:  
   ```bash
   pip install pandas numpy scikit-learn opencv-python matplotlib pillow torch scipy
