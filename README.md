# Wine Quality Prediction using Machine Learning

## Project Overview
This project predicts the quality of red wine using machine learning classification algorithms based on its physicochemical properties.

## Dataset
- Dataset: UCI Wine Quality - Red Wine
- Original records: 1,599
- Records after removing duplicates: 1,359
- Features: 11 physicochemical properties
- Target variable: `quality`
- Missing values: 0

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Data Preprocessing
- Loaded the CSV dataset.
- Checked data types and missing values.
- Identified and removed 240 duplicate rows.
- Explored the distribution of wine quality scores.

## Exploratory Data Analysis
Created visualizations for:
- Wine quality distribution
- Alcohol content versus quality
- Feature correlation heatmap
- Feature importance

## Machine Learning Models
1. Random Forest Classifier
2. Logistic Regression

## Model Performance

| Model | Accuracy |
|---|---:|
| Random Forest | 58.09% |
| Logistic Regression | 41.91% |

Random Forest achieved higher accuracy on the test set. Performance for rare quality scores was weak, so the results should be interpreted with care.

## Sample Prediction
- Actual wine quality: 5
- Predicted wine quality: 5

This sample was predicted correctly. A single correct prediction does not guarantee overall model performance.

## Conclusion
The Random Forest model performed better than Logistic Regression on this train-test split. The dataset contains many more wines with quality scores of 5 and 6 than scores of 3 and 8, which makes predicting rare classes more difficult.

## Project Files
- `winequality-red.csv` — dataset
- `Wine_Quality_Prediction.ipynb` — analysis and machine learning notebook
- `model_comparison.csv` — model accuracy comparison
- `README.md` — project documentation