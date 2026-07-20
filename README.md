# YouTube Video Analytics - Regression Analysis

## About

This project was completed as part of my Machine Learning learning journey. The objective was to understand the complete ML workflow by cleaning a YouTube dataset, performing exploratory data analysis, and building regression models to predict video popularity (like_count).

The project covers the complete pipeline from data preprocessing to model evaluation using Python and Scikit-learn.

---

## Project Workflow

The project is divided into six notebooks:

1. Data Cleaning
   - Handle missing values
   - Remove duplicates
   - Convert YouTube duration to seconds
   - Drop unnecessary columns
   - Save the cleaned dataset

2. Exploratory Data Analysis (EDA)
   - Histograms
   - Boxplots
   - Scatter plots
   - Correlation heatmap
   - Pairplot

3. Simple Linear Regression
   - Predict `like_count` using `view_count`

4. Multiple Linear Regression
   - Predict `like_count` using:
     - `view_count`
     - `comment_count`
     - `duration_seconds`

5. Polynomial Regression
   - Degree 3 polynomial using `view_count`

6. Model Comparison
   - Compare model performance
   - Apply feature scaling
   - Save trained models

---

## Results

| Model | R² Score |
|--------|----------|
| Simple Linear Regression | 0.53 |
| Multiple Linear Regression | 0.52 |
| Polynomial Regression | 0.70 |

Among the three models, Polynomial Regression performed the best on this dataset.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

---

## Running the Project

Clone the repository:

```bash
git clone git@github.com:KartikayCT/Video_Analysis_Project.git
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook and run the notebooks in numerical order from 01 to 06.

---

## Repository Structure

```
notebooks/
processed/
models/
results/
images/
README.md
requirements.txt
youtube_data.csv
```

---

## What I Learned

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Linear and Polynomial Regression
- Model evaluation using MAE, RMSE and R²
- Feature scaling with StandardScaler
- Saving trained models with Joblib

---

## Author

Kartikay Chandra Tiwari

B.Tech Computer Science Engineering

GB Pant Institute of Engineering and Technology

GitHub: https://github.com/KartikayCT