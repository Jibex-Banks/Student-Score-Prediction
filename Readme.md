# Student Performance Predictor

## 📖 Project Overview

This project explores the factors influencing student exam performance through machine learning. By utilizing historical student data, I developed a regression model to predict exam scores based on study habits, attendance, and supplementary tutoring.

The goal of this analysis was to determine which variables hold the most predictive power and to compare the performance of standard Linear Regression against Polynomial Regression models.

## 🛠 Tech Stack

* **Language:** Python
* **Libraries:** `pandas`, `scikit-learn`, `matplotlib`
* **Environment:** Jupyter Notebook / VS Code

## 📊 Key Findings

* **Performance Analysis:** The model shows a strong linear correlation between input features and actual exam scores.
* **Model Experimentation:** * Applied **Linear Regression** as a baseline.
* Evaluated **Polynomial Regression** (degree=2) to identify non-linear relationships.
* Performed **Feature Selection** experiments, observing how removing variables like "Sleep Hours" or "Physical Activity" impacted the $R^2$ score.

### 💡 Key Insights

* **Feature Impact:** Removing "Sleep_Hours" and "Physical_Activity" showed that the model's $R^2$ score was most sensitive to `Hours_Studied` and `Attendance`.
* **Model Comparison:** The Polynomial Regression (degree=2) provided a more nuanced fit for the data compared to the standard Linear Regression, though it also highlighted potential overfitting risks at the extreme ends of the score distribution.
* **Data Observations:**  The scatter plot visualization revealed that while the model is highly effective for average scores, prediction variance increases for high-achieving students, suggesting that non-academic factors might influence top-tier performance.

* **Visualization:** Identified a strong predictive trend, with specific observations on model variance in higher score ranges as seen in the scatter plots.

## 📂 Project Structure

```text
├── StudentPerformanceFactors.csv  # Original dataset
├── analysis.ipynb                 # Jupyter notebook with code and experiments
├── README.md                      # Project documentation
└── requirements.txt               # Dependencies

```

## 🚀 How to Run

1. Clone this repository: `git clone [your-repo-link]`
2. Install the requirements: `pip install -r requirements.txt`
3. Open `analysis.ipynb` to view the data processing and model experimentation.

## 💡 Lessons Learned

This project reinforced the importance of feature selection and data cleaning. It highlighted how even simple models can yield significant insights when provided with high-quality, relevant data.