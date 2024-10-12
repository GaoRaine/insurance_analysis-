# Insurance Charge Prediction

This project explores a dataset containing health-related information aimed at understanding the factors that influence individual medical insurance costs. Using a variety of statistical techniques and machine learning models, we aim to predict medical charges based on attributes such as:

- Age
- Gender
- Body Mass Index (BMI)
- Number of children
- Smoking status
- Geographic region

## Dataset Overview

The dataset contains **1338 observations** and **7 variables**, including:

- **Age**: Age of the individual.
- **Sex**: Gender of the individual (female, male).
- **BMI (Body Mass Index)**: A measure of body fat based on height and weight.
- **Children**: Number of children or dependents covered by insurance.
- **Smoker**: Binary indicator of whether the individual is a smoker (yes, no).
- **Region**: The geographical region where the individual resides (southwest, southeast, northwest, northeast).
- **Charges**: Medical costs incurred by the individual (target variable).

## Research Questions

1. Do smokers incur higher medical charges than non-smokers?
2. Are older individuals more likely to incur higher medical charges?
3. Is there a correlation between higher BMI and medical costs?

## Data Exploration and Visualization

- **Boxplots**: Used to explore the distribution of charges across different categorical variables (sex, smoker, region).


- **Scatter plots**: Visualized relationships between BMI, age, and charges.


- **Correlation Heatmap**: Generated to analyze relationships between numeric variables and charges.

 
## Predictive Modeling

We built a **Multiple Linear Regression Model** to predict medical charges based on the available features. Key insights from the model include:

- **Age**, **BMI**, **number of children**, and **smoking status** have significant effects on medical charges.
- **Smokers** tend to incur significantly higher charges.
- **Age** and **BMI** are positively correlated with medical costs.
- **Region** and **sex** have smaller impacts compared to other variables.

### Model Performance

- **R-squared**: 0.7509, meaning the model explains about 75% of the variability in medical charges.
- **Residual Standard Error (RSE)**: 6062, indicating the average prediction error.

To address non-constant variance and improve the model, a log-transformed model was also explored.

## Hypothesis Testing

We tested three primary hypotheses:

1. **Smokers incur higher medical charges than non-smokers.**
2. **Older individuals incur higher medical charges than younger individuals.**
3. **Individuals with higher BMI incur higher medical charges.**

The results supported all three hypotheses with statistically significant p-values.

## Future Improvements

While the model performs well, we acknowledge some limitations:

- The dataset is relatively small (1338 rows), so the findings may not generalize well to a larger population.
- Additional features, such as health habits or sleeping hours, could further improve the model's predictive power.

## Conclusion

This project provides valuable insights into the factors affecting medical insurance charges. The findings may assist insurance companies in shaping their premium-setting strategies, helping ensure financial stability and equitable services for policyholders.

## How to Run the Code

1. **Clone this repository**.
2. **Load the dataset** using the provided code (`insurance.csv`) under the `data` folder.
3. **Install necessary packages** (listed in `requirements.txt`).
4. **Run the analysis scripts** to replicate the results and visualizations.

---
