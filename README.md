TRAFFIC SIGN CLASSIFICATION (2025)
=========================================================

Overview:
---------
This project aims to classify German traffic signs into one of 43 classes using extracted features. 


Directory Structure:
--------------------
The project is organized as follows:


- train\
    Folder with training image
	- train_metadata.csv
    		Metadata for training images (ids, image filenames and class labels)

- test\
    Folder with test images 
	- test_metadata.csv
    		Metadata for test images (ids, image filenames only, no labels)

- traffic-sign-classification.ipynb
    Python code for this project

- cnn_eval_state.pt
    CNN model trained with weights saved for evaluation
    This is for reproducibility of the test results

- cnn_kaggle_state.pt
    CNN model trained with weights saved for Kaggle test
    This is for reproducibility of the Kaggle test results

- full_cnn_tuning.txt
    CNN model hyperparameter tunning results

- tuned_hyperparameters.txt
    Log file for CNN model training with the chosen set of hyperparameters

- knn_pred.csv
    KNN model predictions for Kaggle test

- random_forest.csv
    Random Forest predictions for Kaggle test

- cnn_pred.csv
    CNN model predictions for Kaggle test

- perspective_transformed.png
    Transformed image for error analysis for Random Forest & CNN

- README.txt
    This file

Data:
-----
- 5488 training images with class labels
- 2353 test images without labels
- 43 total traffic sign classes


Guideline for executing traffic-sign-classification.ipynb:
----------------------------------------------------------
- Python version used for this file: 3.12.7
- Execute all cells in sequential order.
- Cells for hyperparameter tuning can be skipped without causing an error.
- Required external libraries: pandas, numpy, sklearn, cv2, matplotlib, PIL, torch, scipy.

