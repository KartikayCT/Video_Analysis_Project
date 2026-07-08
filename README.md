# YouTube Video Analytics - Regression Analysis

## About the Project

This project was built as part of my Machine Learning learning journey. The objective was to understand the complete machine learning workflow by predicting the **Average View Percentage** of YouTube videos using different regression techniques.

The dataset contains approximately 30,000 YouTube video records with information such as video duration, likes, comments, and viewer engagement.

Instead of focusing only on building models, I also learned how to clean data, explore it visually, evaluate models, apply feature scaling, and save trained models for future use.

---

## Project Goal

The target variable for this project is:

Average View Percentage (`avg_view_percentage`)

Three regression models were built and compared:

- Simple Linear Regression
- Multiple Linear Regression
- Polynomial Regression (Degree = 3)

---

## Project Workflow

### 1. Data Cleaning

The first step was cleaning the dataset before training any model.

Tasks performed:

- Checked for missing values
- Removed duplicate rows
- Dropped unnecessary columns
- Saved the cleaned dataset

---

### 2. Exploratory Data Analysis (EDA)

After cleaning the data, I explored it using different visualizations to understand the relationships between variables.

Some of the plots include:

- Histograms
- Boxplots
- Scatter plots
- Correlation heatmap
- Pair plot

---

### 3. Simple Linear Regression

The first model used only one feature:

- Video Duration

to predict:

- Average View Percentage

This helped me understand how linear regression works with a single independent variable.

---

### 4. Multiple Linear Regression

The second model used three input features:

- Video Duration
- Likes
- Comments

The goal was to check whether adding more information improves prediction accuracy.

---

### 5. Polynomial Regression

Finally, I trained a Polynomial Regression model using only Video Duration with a polynomial degree of 3.

This was done to check whether a non-linear relationship exists between video duration and viewer retention.

---

### 6. Feature Scaling

To understand preprocessing, I also applied **StandardScaler** and compared the model's performance before and after scaling.

---

## Model Performance


 Simple Linear Regression | MAE=24.94 | RMSE=28.78 | R² Score=-0.000058 |
 Multiple Linear Regression | MAE=24.94 | RMSE=28.79 | R² Score=-0.000151 |
 Polynomial Regression | MAE=24.95 | RMSE=28.79 | R² Score=-0.000431 |

---

## Observations

One interesting finding from this project was that none of the three models performed well.

The correlation analysis showed that the selected features had almost no relationship with the target variable. Because of this, even adding more features or using Polynomial Regression did not improve the predictions.

Although the models did not achieve a good R² score, this was an important learning experience because it showed that machine learning models are only as good as the information available in the data.

---

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

---

## How to Run

Clone the repository:

```bash
git clone git@github.com:KartikayCT/Video_Analysis_Project.git
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebooks in the following order:

1. Data Cleaning
2. Exploratory Data Analysis
3. Simple Linear Regression
4. Multiple Linear Regression
5. Polynomial Regression
6. Feature Scaling and Model Analysis

---

## What I Learned

Through this project, I learned how to:

- Clean and preprocess datasets
- Perform exploratory data analysis
- Train regression models using Scikit-learn
- Evaluate models using MAE, RMSE, and R² Score
- Apply StandardScaler
- Understand underfitting and overfitting
- Save trained models using Joblib

---

## Author

Kartikay Chandra Tiwari

B.Tech Computer Science Engineering

GB Pant Institute of Engineering and Technology

GitHub: https://github.com/KartikayCT
