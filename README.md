<h1 align="center">🔥 Digital Burnout Prediction</h1>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue" />
  <img src="https://img.shields.io/badge/ML-User%20Behavior%20Modeling-purple" />
  <img src="https://img.shields.io/badge/XGBoost-F1%3D0.92-green" />
  <img src="https://img.shields.io/badge/Data-1.6M%2B%20logs-orange" />
</p>

---

## 🌟 Overview  
This project detects **Digital Burnout** using large-scale user activity logs.  
With over **1.6 million behavioral events**, we built a high-performance ML pipeline capable of predicting burnout using engineered session-level features and advanced modeling techniques.

A visually clean, efficient, modern ML project designed end-to-end — from data preprocessing to performance evaluation.

---

## 🚀 Key Highlights

- Processed **1.6M+ user behavior logs** (views, cart events, purchases)  
- Engineered **session-level features** without leaking session duration  
- Handled **class imbalance** using **SMOTE**  
- Trained multiple ML models → **XGBoost achieved 92% F1-Score**  
- End-to-end ML pipeline with preprocessing, modeling, and evaluation  
- Clean code, reproducible workflow, high-quality experimentation

---

## 📊 Dataset Summary

| Property | Details |
|---------|---------|
| Total Logs | **1.6 million+** |
| Event Types | view, cart, purchase |
| Processing | Session grouping, interaction ratios, behavior counts |
| Imbalance | Handled using **SMOTE** |
| Location | Add your CSV to `data/2019-Nov.csv` |

⚠ **Dataset not included** (size constraints).  
Place the dataset this way:

data/
└── 2019-Nov.csv


---

## 🧠 ML Pipeline Breakdown

### **1️⃣ Data Processing**
- Aggregated millions of events  
- Grouped by **user_id** + **session**  
- Built interaction-based features  
- Avoided session duration → prevents leakage  
- Normalized + cleaned data  

### **2️⃣ Imbalance Handling**
Used **SMOTE** to oversample minority burnout cases.  
Ensures balanced training for robust model performance.

### **3️⃣ Modeling**
Trained classical and advanced models:

- Logistic Regression  
- Random Forest  
- Decision Tree  
- KNN  
- SVM  
- **XGBoost** (BEST)

### **4️⃣ Evaluation**
| Model | F1-Score |
|-------|----------|
| ⭐ **XGBoost** | ⭐ **0.92** |
| KNN | 0.92 |
| Random Forest | 0.91 |
| SVM | 0.87 |
| Logistic Regression | 0.86 |
| Decision Tree | 0.84 |

📌 **Winner:** **XGBoost (92% F1 Score)**  
Exceptional performance on highly imbalanced sessions.

---

## 📁 Project Structure


Digital_Burnout/
│
├── main.ipynb # End-to-end ML pipeline
├── requirements.txt # Dependencies
├── README.md # Documentation
│
└── data/ # Add dataset here
└── 2019-Nov.csv


---

## 🛠 Tech Stack

**Languages:**  
- Python  

**Libraries:**  
- NumPy  
- Pandas  
- scikit-learn  
- XGBoost  
- imbalanced-learn  
- Matplotlib  
- Seaborn  

**Environment:**  
- Jupyter Notebook  
- VS Code  

---

## ⚙️ Setup & Execution

## 1️⃣ Install Dependencies
pip install -r requirements.txt

## 2️⃣ Run the Notebook
jupyter notebook: main.ipynb

inside the notebook, you'll find:
✔ Data Cleaning
✔ Feature Engineering
✔ SMOTE
✔ Model Training
✔ Evaluation
✔ Comparison plots

## 🎯 Future Enhancements

Add a FastAPI/Flask backend for real-time predictions

Incorporate temporal features with RNN/LSTM

Visualize burnout patterns using SHAP

Integrate with streaming data (Kafka/Spark)

Deploy complete ML pipeline on cloud
