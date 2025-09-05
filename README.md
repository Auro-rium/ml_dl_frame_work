# Machine Learning and Deep Learning Workspace

This repository contains a collection of Jupyter notebooks and scripts for exploring machine learning and deep learning concepts using Python. It covers topics ranging from data preprocessing and feature engineering to training and evaluating machine learning and deep learning models.

## Project Structure

```
ml/
    scikitlearn0.ipynb
    helper_functions.py
    ml_numpy.ipynb
    fundamentals_dl0.ipynb
    fundamentals_dl1.ipynb
    classification_dl2.ipynb
    computervision_dl3.ipynb
data/
    heart-disease.csv
    FashionMNIST/
        raw/
    car-sales-extended.csv
    car-sales-extended-missing-data.csv
models/
    random_forest_model_1.pkl
    random_forest_model_1.joblib
    01_pytorch_fundamentals_model_0.pth
    01_pytorch_workflow_model_1.pth
images/
    numpy-car-photo.png
    numpy-dog-photo.png
    numpy-panda.jpeg
README.md
```

## Contents

### Machine Learning Notebooks
- **`ml/scikitlearn0.ipynb`**:  
  Covers Scikit-learn workflows, including:
  - Data preprocessing (handling missing data, encoding categorical variables).
  - Training and evaluating models like `RandomForestClassifier` and `RandomForestRegressor`.
  - Hyperparameter tuning with `GridSearchCV`.
  - Model persistence using `pickle` and `joblib`.

- **`ml_numpy.ipynb`**:  
  Introduces NumPy basics, including array operations, data manipulation, and image processing.

### Deep Learning Notebooks
- **`fundamentals_dl0.ipynb`** and **`fundamentals_dl1.ipynb`**:  
  Introduce PyTorch fundamentals, including tensor operations, building simple neural networks, and training workflows.

- **`classification_dl2.ipynb`**:  
  Demonstrates classification tasks using PyTorch, including training and evaluating models.

- **`computervision_dl3.ipynb`**:  
  Focuses on computer vision tasks using the FashionMNIST dataset, including data loading, model training, and evaluation.

### Scripts
- **`helper_functions.py`**:  
  Contains reusable utility functions for:
  - Plotting (e.g., loss curves, predictions).
  - Accuracy calculations.
  - Model evaluation.
  - Data downloading and preprocessing.

### Data
- **`heart-disease.csv`**: Dataset for classification tasks.
- **`FashionMNIST/`**: Dataset for computer vision tasks.
- **`car-sales-extended.csv`** and **`car-sales-extended-missing-data.csv`**: Datasets for regression tasks and handling missing data.

### Models
- Pretrained and saved models:
  - `random_forest_model_1.pkl` and `random_forest_model_1.joblib`: RandomForest models trained on car sales data.
  - `01_pytorch_fundamentals_model_0.pth` and `01_pytorch_workflow_model_1.pth`: PyTorch models trained on various tasks.

## Getting Started

1. **Install Dependencies**  
   Ensure you have Python 3.8+ installed. Install the required libraries:
   ```sh
   pip install numpy pandas matplotlib scikit-learn torch torchvision
   ```

2. **Run Notebooks**  
   Open the `.ipynb` files in Jupyter Notebook or Visual Studio Code and execute the cells.

3. **Data Preprocessing**  
   The notebooks include examples of handling missing data, encoding categorical variables, and splitting datasets into training and testing sets.

4. **Model Training and Evaluation**  
   Train machine learning and deep learning models and evaluate their performance using metrics like accuracy, confusion matrix, and cross-validation scores.

5. **Model Persistence**  
   Save and load trained models using `pickle` or `joblib`.

## Key Features

- **Machine Learning**:
  - Classification: Predicting heart disease using `RandomForestClassifier`.
  - Regression: Predicting car prices using `RandomForestRegressor`.
  - Hyperparameter tuning with `GridSearchCV`.
  - Cross-validation for robust model evaluation.

- **Deep Learning**:
  - PyTorch fundamentals: Tensor operations, building and training neural networks.
  - Classification tasks with PyTorch.
  - Computer vision workflows using FashionMNIST.

- **Data Handling**:
  - Handling missing data with techniques like filling and dropping.
  - Encoding categorical variables using `OneHotEncoder` and `ColumnTransformer`.

## License

This project