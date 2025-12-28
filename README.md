## Building Permits Analysis

## Project Overview

This project analyzes building permit data to uncover trends, insights, and patterns, and builds a predictive model to determine the likelihood of permit approval. The work simulates a real-world workflow of a data science internship, involving data cleaning, exploratory data analysis (EDA), visualization, and machine learning modeling. The goal is to provide actionable insights for operational decision-making in construction permit management.

## Key Objectives

Analyze historical building permit data to identify trends by year, neighborhood, and permit type.

Clean and transform raw data for analysis and machine learning.

Develop visualizations to highlight key insights such as top permit types, neighborhood trends, and approval patterns.

Build a predictive model to classify permits as likely approved or rejected based on key features.

## Dataset

Source: Building permits dataset (San Francisco, CA)

Size: 198,900 entries, 43 columns

Key Columns Used:

Permit Type

Filed Date

Issued Date

Zipcode

Estimated Cost

Current Status

Neighborhoods - Analysis Boundaries

## Tools & Technologies

**Programming Languages:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)

**Data Visualization:** Matplotlib, Seaborn, Boxplots, Pie charts, Bar charts

**Data Handling & Analysis:** Pandas, Excel-style operations, date parsing

**Machine Learning:** Random Forest Classifier (scikit-learn)

**Environment:** Google Colab, GitHub for version control

## Process & Workflow

**1. Data Loading & Inspection**

Loaded CSV dataset into Python using Pandas.

Checked column types, missing values, and dataset statistics.

Identified mixed data types and missing values in several columns.

**2. Data Cleaning & Transformation**

Selected relevant columns for analysis.

Handled missing values by filling (Estimated Cost) and dropping rows where essential fields were missing.

Converted date columns to datetime format.

Extracted Year and Month from relevant date columns for trend analysis.

3. Exploratory Data Analysis (EDA)

Visualized number of permits issued per year to identify temporal trends.

Analyzed top 10 permit types and neighborhoods by permit count.

Created bar plots, pie charts, and boxplots for categorical and numerical variables.

Investigated estimated costs across permit types using boxplots.

4. Feature Engineering

Converted Current Status into a binary target variable (Approval) for machine learning:

Issued → 1 (Approved)

Others → 0 (Not Approved)

Selected key features for model training: Zipcode, Year, Estimated Cost.

5. Machine Learning Modeling

Split dataset into training (80%) and testing (20%) sets.

Trained a Random Forest Classifier to predict permit approval.

Evaluated the model using accuracy and classification report.

Achieved high accuracy in classification tasks.

## Results & Insights

The number of building permits fluctuates across years, showing trends influenced by city development.

Certain neighborhoods consistently have higher permit activity.

Estimated cost varies significantly across permit types, with new construction and additions showing higher costs.

Random Forest Classifier successfully predicts permit approval with high accuracy.

## Conclusion

This project demonstrates the end-to-end workflow of a data science internship:

Data cleaning, preprocessing, and transformation for analysis.

Visualization and trend analysis to generate actionable insights.

Application of machine learning to solve a practical classification problem.

The project highlights the ability to handle large datasets, identify operational trends, communicate results visually, and build predictive models for real-world business use cases.
