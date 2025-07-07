# rural-electrification-flfp
An exploratory regression project on female labor force participation and rural electrification using simulated NFHS data.
 Rural Electrification and Female Labor Force Participation (FLFP)

📊 This is an independent exploratory project estimating the effect of rural electrification on female labor force participation in India, using simulated NFHS-style data and OLS regression in Python.

🔍 Objective

To understand whether access to electricity is associated with increased labor force participation among women in rural households.

 📁 Project Structure

rural-electrification-flfp/
├── data/
│ └── raw/ # Sample cleaned dataset (nfhs_sample_cleaned.csv)
├── notebooks/
│ └── 01_data_exploration.ipynb # Full data prep and regression analysis
├── output/
│ └── regression_summary.csv # Model output table
├── .gitignore
└── README.md

 🧪 Methodology

- Data loaded and pre-processed using `pandas`
- OLS regression with `statsmodels`
- Controlled for: age, education level, caste, and state fixed effects
- Cleaned categorical variables with one-hot encoding
- Converted all data to numeric before modeling

 Sample Model:

```python
model = sm.OLS(y, X).fit()
model.summary()


📌 Key Finding
Electrification was not statistically significant in predicting FLFP in this simulated dataset. However, caste and education showed stronger associations. More detailed modeling is needed with real household-level data.

📦 Tools Used
Python: pandas, statsmodels, matplotlib, jupyter

Git & GitHub for version control

VS Code for development

🧑‍💻 About the Author
This project is part of my transition into economics research. I am preparing for RA roles and PhD applications, and this repository serves as a public portfolio of my coding and research capabilities.

