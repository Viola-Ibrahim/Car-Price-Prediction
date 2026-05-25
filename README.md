# Car-Price-Prediction

A machine learning project focused on predicting car prices based on technical specifications and vehicle characteristics.

## Project Overview

This project explores the factors that influence car prices and builds a regression model capable of estimating vehicle prices based on multiple features such as engine size, horsepower, fuel efficiency, and brand information.

The workflow includes:

- Data exploration and visualization
- Data cleaning and preprocessing
- Outlier detection and handling
- Feature engineering
- Correlation analysis
- Model training and evaluation
- Performance interpretation and insights

---

## Dataset

The dataset contains various car specifications, including:

- Car name
- Brand
- Engine size
- Horsepower
- Curb weight
- Fuel efficiency (city/highway MPG)
- Body type
- Fuel type
- Price

---

## Data Preprocessing

Several preprocessing steps were applied to improve data quality and model performance:

- Checked for missing values and duplicates
- Detected and handled outliers using clipping
- Encoded categorical variables
- Extracted **Brand** from `CarName` as a new feature
- Removed highly correlated features to reduce multicollinearity
- Applied feature scaling where necessary
- Used log transformation on the target variable to reduce skewness and improve stability

---

## Exploratory Data Analysis (EDA)

Key visualizations included:

- Price distribution
- Feature correlation heatmaps
- Boxplots for outlier detection
- Scatterplots of important numerical features
- Actual vs Predicted price comparison

---

## Model Building

A regression model was trained to predict car prices.

### Evaluation Metrics

| Metric | Train | Test |
|--------|-------|------|
| R² Score | 0.9426 | 0.8857 |
| MSE | 0.0143 | 0.0295 |
| MAE | 0.0940 | 0.1300 |

---

## Key Insights

- **Engine size and curb weight** showed the strongest positive correlation with car price.
- **Horsepower** was also a significant predictor of price.
- **Fuel efficiency** had a negative relationship with price, suggesting that more expensive cars often prioritize performance over economy.
- **Brand information** improved predictive power significantly after feature engineering.
- The model achieved strong predictive performance with **minimal overfitting**, indicating good generalization on unseen data.

---

## Final Conclusion

The analysis showed that car price is mainly influenced by factors related to **vehicle size, performance, and brand identity**.

After preprocessing, feature engineering, and careful handling of outliers, the final model achieved strong performance with an **R² score of approximately 0.89** on the test set.

---

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Repository Structure

```bash
├── CarPrice.ipynb
├── README.md
└── dataset.csv
```

---

## Author

**Viola Ibrahim**  
Computer Science student passionate about machine learning, problem solving, and building practical data-driven projects.
