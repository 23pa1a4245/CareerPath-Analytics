# CareerPath Analytics

CareerPath Analytics is a data analytics and machine learning project developed as part of the HCL Data Analytics program.

The project analyzes employee and career-related data to support career guidance, workforce planning, and employee attrition analysis.

## Features

1. **Executive Overview** – Key workforce metrics and dataset quality indicators.
2. **Career Progression** – Explore employee career and job-related patterns.
3. **Workforce Planning** – Analyze workforce distribution and trends.
4. **ML Attrition Lab** – Predict employee attrition using machine learning models.
5. **Recommendations & Limitations** – Present data-driven insights and discuss model limitations.
6. **Career Assistant** – Explore career-related insights using the available dataset.

## Technology Stack

- Python
- Streamlit
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Joblib

## Machine Learning

The project compares:
- Logistic Regression
- Random Forest

The model training process uses grouped splitting to prevent identical employee profiles from appearing in both training and testing sets.

## Dataset Information

The project uses an IBM HR Analytics-style employee dataset.

**Important limitation:** The expanded dataset contains resampled employee profiles. Although employee IDs are unique, many employee profiles repeat. These repeated records are not independent employee observations. Therefore, model evaluation results are educational and should not be interpreted as proof of real-world predictive performance.

The dataset is not included in this repository. Place a compatible dataset named `hr_data.csv` in the project root before running the application or training the models.

## Installation and Setup

Clone the repository:

```bash
git clone https://github.com/23pa1a4245/CareerPath-Analytics.git
cd CareerPath-Analytics
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Add your compatible `hr_data.csv` file to the project folder.

Train the models:

```bash
python train_model.py
```

Run the Streamlit application:

```bash
streamlit run app.py
```

## Project Structure

```text
CareerPath-Analytics/
│
├── app.py
├── train_model.py
├── check_data_quality.py
├── expand_dataset.py
├── requirements.txt
├── README.md
├── PROJECT_REPORT_TEMPLATE.md
├── UPGRADE_STEPS.txt
├── VIVA_QUESTIONS.md
└── models/
```

## Disclaimer

This project is intended for educational and analytical purposes. Predictions should not be used as the sole basis for employment or workforce decisions.