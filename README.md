# Image Classification using Support Vector Machine (SVM)
This project implements an image classification system that uses a Support Vector Machine (SVM) to classify images into two categories: empty and not_empty. The classifier is trained on a dataset of images, using a grid search to optimize the SVM's hyperparameters. The model can then be used to predict unseen images in these two categories.

## Features
1. Image Preprocessing: Resize images to a smaller dimension for efficient model training.
2. SVM Classification: Uses SVM for binary classification (empty vs not_empty).
3. Hyperparameter Tuning: Grid search is used to find the best parameters for the SVM.
4. Model Persistence: Saves the trained model using pickle for future use.
## Files in the Repository
--> main.py: The main Python script that processes images, trains the SVM model, and evaluates it.\
--> model.p: The serialized SVM model saved after training, which can be loaded and used for prediction.\
--> dataset/: Directory containing the images classified into empty and not_empty categories (to be created/added by the user).
## Installation
### Prerequisites
Python 3.x
### Required Python libraries:
scikit-learn\
numpy\
scikit-image\
pickle
## Steps to Run
-Clone the repository:
### git clone https://github.com/FariaRaghib/Image Classification using Support Vector Machine (SVM)
### cd Image Classification using Support Vector Machine (SVM)
-Install the required Python packages:
### pip install scikit-learn numpy scikit-image
-Set up the dataset:
The dataset should be organized into two folders (empty and not_empty) within the dataset/ directory. Each folder should contain relevant images.
-Run the script:
### python main.py
The script will:
- Load the images from the dataset/ directory.
- Preprocess the images (resize and flatten).
- Split the data into training and testing sets.
- Train the SVM model using grid search.
- Save the trained model as model.p.
Once the script finishes, you will see the classification accuracy printed to the console, and the model will be saved as model.p.

## How It Works
-Data Preparation: Images are loaded from two categories (empty and not_empty) and resized to 15x15 pixels.\
-Training: A Support Vector Machine (SVM) classifier is trained using grid search to optimize parameters.\
-Evaluation: The accuracy of the classifier is evaluated using a test set.\
-Model Saving: The best model is saved as model.p for later use.\\
