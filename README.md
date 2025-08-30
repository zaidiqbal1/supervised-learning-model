# Supervised Learning with Hyperparameter Tuning

## 📊 Dataset Description
- The dataset used in this project is located at:  
  `/content/drive/MyDrive/train_data.csv`
- It contains preprocessed features and a target column for supervised learning tasks.
- Features (`X`) are used for training, while the target (`y`) represents the output variable (classification or regression).

---

## 🤖 Models Trained
We experimented with the following supervised learning models:
- **Classification Models**
  - Logistic Regression
  - Random Forest Classifier
- **Regression Models**
  - Linear Regression
  - Decision Tree Regressor

---

## ⚙️ Hyperparameter Tuning
To optimize model performance, we used:
- **GridSearchCV** – Exhaustive search over parameter combinations  
- **RandomizedSearchCV** – Random parameter combinations with faster results  

Parameters tuned include:
- Logistic Regression → Regularization strength (`C`), solver  
- Random Forest → Number of estimators (`n_estimators`), max depth, min samples split  
- Decision Tree → Max depth, min samples split, criterion  

Cross-validation (CV=5) was applied to ensure generalization.

---

## 📈 Evaluation Results and Observations

### Classification
- Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix  
- Best model (example): **Random Forest Classifier**  
  - Accuracy: `0.92`  
  - Precision: `0.90`  
  - Recall: `0.91`  
  - F1-score: `0.90`

### Regression
- Metrics: Mean Squared Error (MSE), Root Mean Squared Error (RMSE), R² Score  
- Best model (example): **Decision Tree Regressor**  
  - MSE: `12.3`  
  - RMSE: `3.5`  
  - R² Score: `0.88`

---

## 🛠️ How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/<your-username>/supervised-learning-model.git
   cd supervised-learning-model
