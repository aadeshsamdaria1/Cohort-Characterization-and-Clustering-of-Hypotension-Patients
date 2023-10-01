# Assignment 2 - Cohort characterisation and clustering
# COMP90089 - Machine Learning Applications for Health
# Aadesh Samdaria
# Student ID: 1363757
# Email: asamdaria@student.unimelb.edu.au

## Problem Description:
The dataset containing information about patients with profound hypotension. The dataset includes the following columns:
- ID: Patient de-identified number
- anchor_age: Age of the patient (years)
- gender: F for female and M for male
- dod: Date of Death (if empty, the patient survived - patient outcome variable)
- apsiii: Severity of illness score
- LoS: Length of stay in ICU (days - patient outcome variable)
- charlson_comorbidity_index: Co-morbidity index
The goal is to find subgroups of patients that can have similar charcteristics. This can be useful to predict the mortality rate and other outcomes of a new patient. 

## Problem Solution:
The probelem solution is devided into 3 parts:

- Part 1: EDA: Study and describe the main properties of the profound hypotension cohort using summary statistics and visualizations.

- Part 2: Clustering: Perform k-means clustering to identify subgroups of patients. Use the elbow method to determine an appropriate number of clusters. Select two different values of k for further analysis.

- Part 3: Interpretation: Analyze the main property differences between the clusters and investigate their relation to patient outcomes. Provide visualizations to support findings.

## Files and Notebooks required:
- COMP90089_assignment2_1363757_environment.yaml
- COMP90089_assignment2_1363757_notebook.ipynb
- hypotension_patients.csv

## Instructions to recreate the environment:

## Core packages and versions:
- Pandas version: 1.5.3
- Matplotlib version: 3.7.0
- Seaborn version: 0.12.2
- Scikit-learn version: 1.2.1

## References:
- Ahlqvist, E., Storm, P., Käräjämäki, A., Martinell, M., Dorkhan, M., Carlsson, A., Vikman, P., Prasad, R.B., Aly, D.M., Almgren, P. and Wessman, Y., 2018. Novel subgroups of adult-onset diabetes and their association with outcomes: a data-driven cluster analysis of six variables. The lancet Diabetes & endocrinology, 6(5), pp.361-369.
- Roffman, C., Buchanan, J. and Allison, G., 2016. Charlson comorbidities index. Journal of physiotherapy, 62(3).


