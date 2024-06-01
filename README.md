# Employee Retention Analysis

## Project Overview

This repository contains the analysis of employee retention based on a dataset consisting of various parameters such as satisfaction level, number of projects, average monthly hours, and other factors. The analysis is performed using Python, with a strong emphasis on exploratory data analysis (EDA), data visualization, and model creation.

## Data Overview

The dataset consists of 10 columns and 14,999 entries with the following key columns:
- `satisfaction_level`: Level of employee satisfaction
- `last_evaluation`: Last employee evaluation score
- `number_project`: Number of projects handled
- `average_montly_hours`: Average monthly hours worked
- `time_spend_company`: Number of years spent in the company
- `Work_accident`: Whether the employee had a work accident (1: Yes, 0: No)
- `promotion_last_5years`: Whether the employee was promoted in the last 5 years (1: Yes, 0: No)
- `salary`: Employee salary level (low, medium, high)
- `left`: Whether the employee left the company (1: Yes, 0: No)

## Methodology

1. **Exploratory Data Analysis (EDA):**
   - Visualization of data using Seaborn and Matplotlib.
   - Analysis of factors affecting employee retention such as satisfaction level, work accidents, and salary.

2. **Data Cleaning:**
   - Handling missing values, particularly in the `satisfaction_level` column by substituting with the mean value.
   - Conversion of categorical values to numerical representations using ordinal mapping.

3. **Data Visualization:**
   - Usage of plots like countplots, boxplots, and histograms to explore different aspects of the data.
   - Insights drawn from visualizations highlighting areas like satisfaction levels, number of projects, and last evaluations.

## Key Findings

- The average satisfaction level among employees is approximately 0.61.
- Employees spend around 201 average monthly hours, with an average tenure of 3.5 years at the company.
- Approximately 24% of the employees have left the organization, with low satisfaction levels being a significant factor.
- Work accidents are relatively low, observed in around 14.5% of cases.
- Promotions in the last 5 years are rare, around 2%.

## Model Creation and Evaluation

1. **Data Preprocessing:**
   - Dropping irrelevant columns and handling missing data.

2. **Dataset Split:**
   - Splitting the dataset into training and test sets with an 80-20 ratio.

3. **Model Selection:**
   - Using XGBoost and Random Forest classifiers.
   - Hyperparameter tuning with GridSearchCV.

4. **Model Training:**
   - Training the XGBoost model with specific parameters achieving an accuracy of 99.17% on the test set.

5. **Model Evaluation:**
   - Using confusion matrix and heatmap for evaluation.

## Conclusion

This comprehensive analysis provides insights into the factors influencing employee retention. The data-driven approach and robust model help in understanding the key parameters affecting employee turnover, which can aid in developing strategies for improvement.

## Getting Started

To explore the analysis:
1. Clone this repository.
2. Install necessary dependencies using `pip install -r requirements.txt`.
3. Execute the Jupyter Notebook or Python scripts provided.

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to the contributors of the data and the open-source community for their tools and libraries.
