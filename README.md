# Customer Churn Prediction

This project predicts whether a telecom customer is likely to churn using the IBM Telco Customer Churn dataset. It includes data preprocessing, exploratory analysis, model comparison, and a Streamlit app that scores customer risk in real time.

## Highlights
- Data cleaning and preprocessing for numeric and categorical features
- Exploratory analysis of churn drivers and customer patterns
- Model comparison using Logistic Regression and Random Forest
- Final Random Forest model saved for deployment
- Interactive Streamlit dashboard for churn prediction

## Project structure
- `IBM Telco Customer churn.csv` — telecom customer dataset
- `notebook.ipynb` — model development and evaluation
- `Churn_app.py` — Streamlit web app
- `final_rf.pkl` — trained Random Forest model
- `encoder.pkl` — categorical encoder
- `scaler.pkl` — feature scaler
- `feature_names.pkl` — model feature order
- `reports/` — project reports and visualizations

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run Churn_app.py
```

## How to use
1. Start the Streamlit app.
2. Enter customer details such as tenure, charges, services, and contract type.
3. Click `Predict Churn`.
4. Review the predicted churn label and churn probability.

## Technologies
- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- Streamlit

## Priority improvements
1. Evaluate the model properly: report churn precision/recall, F1, ROC-AUC, and PR-AUC—not accuracy alone.
2. Tune for your goal: use cross-validation and choose a prediction threshold that balances missed churners against false alarms.
3. Compare stronger models: try XGBoost, LightGBM, or CatBoost against your current models.
4. Polish the app: show clear risk levels and explain the main factors behind each prediction.
5. Make it reproducible: add basic tests, document setup and limitations, and organize the training and app code. 


## License
This project is licensed under the MIT License.
