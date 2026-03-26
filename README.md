# Synthetic Student Dropout Dataset

This repository contains a synthetic dataset designed for a Machine Learning project about **student dropout prediction**.  
The dataset simulates demographic, academic, and financial information from university students, along with a target variable indicating whether the student dropped out.

## Project Purpose

The goal of this dataset is to support an academic activity focused on:

- Comparing supervised and unsupervised learning
- Building a binary classification model
- Predicting student dropout using historical-style data
- Practicing synthetic dataset generation in Python

## Dataset Description

The dataset contains **500 records** and includes the following variables:

| Variable | Type | Description | Range / Categories |
|---------|------|-------------|---------------------|
| `student_id` | Integer | Unique identifier for each student | 1 to 500 |
| `age` | Integer | Student age | Usually 16 to 29, with some outliers |
| `gender` | Categorical | Student gender | Male, Female |
| `origin` | Categorical | Place of origin | Urban, Rural |
| `high_school_avg` | Numeric | High school average grade | 2.0 to 5.0 |
| `admission_score` | Numeric | Admission test score | 0 to 100 |
| `first_semester_grade` | Numeric | First semester grade | 0.0 to 5.0 |
| `socioeconomic_level` | Integer | Socioeconomic level | 1 to 5 |
| `scholarship` | Categorical | Whether the student has a scholarship | Yes, No |
| `loan` | Categorical | Whether the student has a loan | Yes, No |
| `dropout` | Categorical | Target variable | Yes, No |

## Target Variable

The output variable is:

- `dropout = Yes`
- `dropout = No`

This variable represents whether a student is at risk of leaving the university.

## How the Dataset Was Generated

The dataset was created using Python and pandas in Google Colab.  
The values were generated synthetically to resemble a realistic university dropout scenario.

The target variable was built using a simple rule based on academic and socioeconomic risk factors, such as:

- Low first semester grades
- Low high school averages
- Low socioeconomic level

Some randomness was added to make the dataset less deterministic and more realistic for machine learning practice.

## Missing Values

To simulate real-world data problems, missing values were introduced intentionally.

- Around **5%** of the values in selected columns were replaced with `NaN`
- This helps test how models and preprocessing steps handle incomplete data

## Outliers

Outliers were also added to simulate unusual or incorrect values that may appear in real datasets.

Examples include:

- Very high `first_semester_grade` values such as `10.0`
- Very low `admission_score` values such as `-15.0`
- Extreme `age` values such as `5` or `60`

These outliers are useful for practicing data cleaning and preprocessing.

## Data Types

- **Numeric variables:** `age`, `high_school_avg`, `admission_score`, `first_semester_grade`, `socioeconomic_level`
- **Categorical variables:** `gender`, `origin`, `scholarship`, `loan`, `dropout`
- **Identifier variable:** `student_id`

## Files

- `synthetic_student_dropout_dataset.csv` → main dataset file
- `README.md` → dataset description and generation details

## How to Use

You can use this dataset for:

- Exploratory Data Analysis
- Data cleaning practice
- Classification model training
- Feature engineering
- Comparing machine learning algorithms

## Example Use Case

A university could use this kind of dataset to build a predictive model that identifies students who may need academic or financial support early in the semester.

## Notes

- This is a **synthetic** dataset, not real student data.
- It was created only for academic and demonstration purposes.
- The dataset includes intentional imperfections such as missing values and outliers.

## Authors

- Arturo Mendoza
- Course: Data Mining
- Activity 1: Supervised vs. Unsupervised Learning
