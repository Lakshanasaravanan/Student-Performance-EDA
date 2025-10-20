# Student Performance Analysis

## Project Overview
This project focuses on analyzing and predicting student academic performance using data-driven approaches.  
The analysis is based on the **UCI Student Performance Dataset**, which includes information about students’ demographics, social background, and study-related factors.

The primary goal is to identify the key factors influencing student outcomes and build a machine learning model to predict their academic performance in both **theory and practical assessments**.

## Objectives
- To analyze various factors affecting student performance.  
- To predict students’ final grades based on behavioral and academic indicators.  
- To visualize trends between theory and practical performance.  


##Dataset Information
**Dataset Source:** [UCI Machine Learning Repository – Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/Student+Performance)

The dataset consists of two CSV files:
- `student-mat.csv` → Mathematics performance  
- `student-por.csv` → Portuguese language performance  

**Key Columns:**
- `G1` – First period grade (*interpreted as Theory Performance*)  
- `G2` – Second period grade (*interpreted as Practical Performance*)  
- `G3` – Final grade (*Overall performance*)  

Additional features include:
- **Demographic factors:** age, gender, address type  
- **Academic factors:** study time, failures, absences  
- **Social factors:** family support, parental education, alcohol consumption  

## Methodology

1. **Data Loading & Cleaning**
   - Imported both datasets and merged them.
   - Handled missing values and encoded categorical features.

2. **Exploratory Data Analysis (EDA)**
   - Generated summary statistics and correlation heatmaps.
   - Visualized the relationship between study habits, absences, and grades.

3. **Feature Engineering**
   - Selected relevant features impacting academic results.
   - Scaled and normalized data for model performance.

4. **Model Building**
   - Implemented machine learning algorithms:
     - Linear Regression  
     - Decision Tree Regressor  
     - Random Forest Regressor  
   - Target variable: `G3` (final grade)

5. **Model Evaluation**
   - Evaluated performance using:
     - R² Score  
     - Mean Absolute Error (MAE)  
     - Mean Squared Error (MSE)

6. **Visualization**
   - Created charts showing correlations and feature importance using **Matplotlib** and **Seaborn**.

##  Tools & Technologies
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Environment:** Google Colab / Jupyter Notebook  

##  Results & Insights
- Study time, parental education, and absences are major predictors of student success.  
- Students with higher study time and family support tend to achieve better results.  
- The **Random Forest Regressor** achieved the best prediction accuracy among the models tested.
