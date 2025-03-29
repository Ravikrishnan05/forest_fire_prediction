# Forest Fire area Prediction

## 📌 Project Overview
This project focuses on predicting forest fire occurrences using machine learning models. We utilize the **Forest Fire Prediction Dataset** and apply various regression techniques to evaluate their effectiveness in predicting fire intensity.

## 📂 Dataset
- The dataset contains multiple environmental and meteorological features.
- Features include **temperature, humidity, wind speed, and other atmospheric conditions**.
- The target variable represents the **fire intensity or area burned**.

## 🛠️ Preprocessing
- **Principal Component Analysis (PCA)** was applied for dimensionality reduction.
- The dataset was split into **training (80%) and testing (20%)**.
- Standardization was performed using **StandardScaler**.

## 📊 Models Implemented & Performance Metrics
We trained multiple regression models and evaluated them using **Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R² Score**.

| Model                     | MSE    | RMSE   | MAE    | R² Score |
|---------------------------|--------|--------|--------|----------|
| Linear Regression         | 11779.35 | 108.53 | 25.04 | 0.0007 |
| ElasticNet                | 11787.90 | 108.57 | 24.66 | -0.00001 |
| Lasso                     | 11782.64 | 108.54 | 24.82 | 0.0004 |
| Ridge Regression          | 11779.38 | 108.53 | 25.03 | 0.0007 |
| Decision Tree             | 17555.13 | 132.49 | 28.55 | -0.4892 |
| Random Forest             | 14485.58 | 120.35 | 26.18 | -0.2288 |
| Gradient Boosting         | 17282.90 | 131.46 | 30.35 | -0.4661 |
| Support Vector Regression | 12154.79 | 110.24 | 19.59 | -0.0311 |
| Kernel Ridge Regression   | 12481.89 | 111.72 | 25.51 | -0.0588 |

The **Linear Regression** model was selected as the best-performing model.

## 📈 Visualization & Evaluation
- **Cumulative Accuracy Profile (CAP) Curve** was used to compare model performance.
- **ROC-AUC Score** was computed for classification performance.
- **Residual Plots** were generated to analyze error distribution.

## 🔍 Key Findings
- Linear Regression performed slightly better in terms of R² score.
- More complex models like Random Forest and Gradient Boosting did not show significant improvements.
- Feature selection and hyperparameter tuning can further enhance accuracy.

## 🚀 Future Improvements
- Implement **Deep Learning models (ANN, CNNs)** for enhanced performance.
- Use **Feature Engineering** to extract more relevant attributes.
- Apply **Hyperparameter Optimization** using GridSearchCV or Bayesian Optimization.

## 📜 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/forest-fire-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the main script:
   ```bash
   python main.py
   ```

## 📢 Contributions & Feedback

Contributions and suggestions are welcome! Feel free to open an issue or submit a pull request. 🚀
