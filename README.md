# 🛍️ Online Shoppers Purchase Prediction

This project uses machine learning to predict whether an online shopping session ends in a purchase (conversion) based on user behavior data.

## 📂 Dataset

- **Name**: Online Shoppers Intention
- **Source**: UCI Machine Learning Repository
- **Size**: 12,330 records
- **Features**: 17 attributes including Month, Weekend, Page durations, Bounce rates, and VisitorType

## 🎯 Objective

To build a classification model that predicts whether a user will make a purchase (`Revenue`) or not, using behavioral and technical features.

## 🧠 Machine Learning Pipeline

1. **Data Cleaning**
   - Converted boolean fields to integers
   - Engineered `Returning_Visitor` feature
   - Encoded categorical `Month` using OrdinalEncoder

2. **Preprocessing**
   - Handled missing values using `SimpleImputer`
   - Normalized features using `MinMaxScaler`

3. **Feature Selection**
   - Selected top 6 features using `SelectKBest` with `chi2`

4. **Modeling**
   - Tried multiple classifiers
   - Final model used: **Support Vector Classifier (SVC)**

5. **Evaluation Metrics**
   - **Accuracy**: 89%
   - **F1 Score**: 52% for class 1 (purchase)
   - **ROC AUC**: 76%

## 🛠️ Technologies Used

- Python 3
- pandas, numpy
- scikit-learn
- matplotlib / seaborn (optional for visualization)

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-github-username>/online-shoppers-prediction.git

# 2. Navigate to the project folder
cd online-shoppers-prediction

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the script
python online_shoppers_prediction.py
```

## 📈 Sample Output
```
              precision    recall  f1-score   support

           0       0.90      0.98      0.94      3127
           1       0.75      0.39      0.52       572

    accuracy                           0.89      3699
   macro avg       0.83      0.68      0.73      3699
weighted avg       0.88      0.89      0.87      3699
```

## 👤 Author

**Kishore Reddy**  
📧 kishorereddy5208@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/kishorereddy-ai)

---

Feel free to ⭐ star this repository if you found it useful!
