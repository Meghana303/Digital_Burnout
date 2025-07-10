#  Digital Burnout Prediction

This machine learning project predicts digital burnout based on user session behavior. The dataset is preprocessed, balanced using SMOTE, and evaluated using multiple classification models.

 **Dataset Note:**  
Due to size limitations, the CSV file is not uploaded here.  
You can manually place it inside a `data/` folder as `2019-Nov.csv`.

## How to Run
1. Install requirements: pip install -r requirements.txt

2. Open `main.ipynb` using Jupyter Notebook.

## Models Evaluated
- Logistic Regression
- Random Forest
- Decision Tree
- KNN
- SVM
- XGBoost

## Final Chosen Models
 XGBoost — F1: 0.93  
 KNN — F1: 0.92  
 Random Forest — F1: 0.91

