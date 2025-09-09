# Rainfall Prediction using Machine Learning – Python

## Overview
This project predicts the possibility of rainfall for a given day using historical weather data.  
It uses data preprocessing, visualization, feature engineering, and machine learning algorithms to build a robust prediction model.

---

## Objective
To develop a reliable model that predicts **rainfall occurrence** based on daily weather conditions.  
Potential applications include:
- 🌾 Agriculture & irrigation planning  
- 🌊 Water resource management  
- ⚠ Disaster prevention & preparedness  
- ☀ Everyday decision making  

---

## Technologies Used
- **Python**  
- **Libraries:**
  - Pandas, NumPy – Data handling
  - Matplotlib, Seaborn – Visualization
  - Scikit-learn – Machine learning algorithms & metrics
  - XGBoost – Gradient boosting classifier
  - imbalanced-learn – Handling imbalanced datasets

---

## 📂 Project Workflow
1. **Data Loading & Cleaning**
   - Removed extra spaces in column names  
   - Filled missing values with column mean  

2. **Exploratory Data Analysis (EDA)**
   - Distribution plots  
   - Box plots for outlier detection  
   - Correlation heatmap  

3. **Feature Engineering**
   - Removed highly correlated and redundant features  
   - Encoded target labels (`yes` → 1, `no` → 0)  

4. **Handling Imbalanced Data**
   - Used `RandomOverSampler` to oversample minority class  

5. **Model Training**
   - Logistic Regression  
   - XGBoost Classifier  
   - Support Vector Classifier (SVC)  

6. **Model Evaluation**
   - ROC-AUC Score  
   - Confusion Matrix  
   - Classification Report  

---

## 📊 Results
| Model                  | Train ROC-AUC | Validation ROC-AUC | Validation Accuracy |
|------------------------|--------------:|-------------------:|--------------------:|
| Logistic Regression    | 0.8893        | 0.8967              | ~89%                |
| XGBoost Classifier     | 1.0000        | 0.8391              | ~84%                |
| Support Vector Classifier (SVC) | 0.9026        | 0.8858              | **85%**             |

Final Model Chosen: **SVC**  
**Validation Accuracy:** **85%**  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Rainfall-Prediction-using-Machine-Learning---Python.git

Navigate to the project directory:
cd Rainfall-Prediction-using-Machine-Learning---Python

Install the required packages:
pip install -r requirements.txt

Run the script:
python rainfall_prediction.py

## Dataset
<br>
The dataset (Rainfall.csv) contains daily weather measurements such as:

Pressure, temperature, dew point

Humidity, cloud cover, sunshine hours

Wind direction, wind speed

Rainfall occurrence (Yes/No)
