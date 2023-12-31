# Cohort Characterization and Clustering of Hypotension Patients

## Problem Description:
The dataset contains information about patients with profound hypotension. The dataset includes the following columns:
- ID: Patient de-identified number
- anchor_age: Age of the patient (years)
- gender: F for female and M for male
- dod: Date of Death (if empty, the patient survived - patient outcome variable)
- apsiii: Severity of illness score
- LoS: Length of stay in ICU (days - patient outcome variable)
- charlson_comorbidity_index: Co-morbidity index
The goal is to find subgroups of patients that can have similar characteristics. This can be useful to predict the mortality rate and other outcomes of a new patient.  <br>


**Importance:** Hypotension is a severe medical condition characterized by abnormally low blood pressure. Hypotension can lead to various life-threatening complications. Therefore, it is crucial for healthcare professionals to promptly diagnose patients and develop treatment plans while efficiently allocating medical resources.<br>

**Obstacles:** The challenges include detecting missing data and outliers within the dataset, determining an appropriate value for 'k' in clustering analysis, and validating the choice of 'k' through alternative methods. Additionally, identifying the common characteristics of patients within distinct subgroups is a significant challenge.<br>

Note: Outlier detection was not included in the submission as all attribute values in the dataset fell within the valid range for each specific attribute. <br>

## Problem Solution Overview:
The problem solution is divided into 3 parts:

- Part 1: EDA (Exploratory Data Analysis): Study and describe the main properties of the profound hypotension cohort using summary statistics and visualizations.

- Part 2: Clustering: Perform k-means clustering to identify subgroups of patients. Use the elbow method to determine an appropriate number of clusters. Select two different values of k for further analysis.

- Part 3: Interpretation: Analyze the main property differences between the clusters and investigate their relation to patient outcomes. Provide visualizations to support findings.

The details of the solution are present in the notebook.

## Files and Notebooks Required:
- environment.yaml - Environment file
- cohort-characterization-and-clustering.ipynb - Notebook(Solution)
- hypotension_patients.csv (Dataset)

## Core Packages and Versions:
- Pandas version: 1.5.3 - [Pandas](https://pandas.pydata.org/)
- Matplotlib version: 3.7.0 - [Matplotlib](https://matplotlib.org/)
- Seaborn version: 0.12.2 - [Seaborn](https://seaborn.pydata.org/)
- Scikit-learn version: 1.2.1 - [Scikit-learn](https://scikit-learn.org/stable/)

## Instructions to Recreate the Environment:
### Method 1:
- Ensure all the files mentioned above are in the same directory.
- Make sure Anaconda is installed on the system ([Download link](https://www.anaconda.com/download))
- Open Anaconda prompt. This is the Anaconda command-line interface.
- Execute this command: `conda env create -f COMP90089_assignment2_1363757_environment.yaml` 
    This will recreate the environment. It will take a couple of minutes to recreate the environment. Change the path of the environment file if needed.
- Open Anaconda and then change the environment to 'Environment_1363757.' or run the command: `conda activate Environment_1363757`
- Launch Jupyter Notebook.
- Click on 'COMP90089_assignment2_1363757_notebook.ipynb' to open the notebook and execute the notebook. Change the path of the hypotension_patients.csv file if needed.

### Method 2:
This method is the fallback method.
If there was an issue in creating the environment, open Anaconda, and in the default environment, manually install the core packages and versions through the UI or using a command. 
The packages can be installed using the command :`conda install pandas=1.5.3 matplotlib=3.7.0 seaborn=0.12.2 scikit-learn=1.2.1`

### Method 3:
- This method is an alternative fallback method.
- Go to Google Colab: Open a web browser and go to Google Colab.
- Click on "File" > "Upload Notebook" and upload the notebook file COMP90089_assignment2_1363757_notebook.ipynb from your local system.
- Upload the dataset file hypotension_patients.csv to Google Colab using the "Files" tab in the left sidebar.
- Install Required Libraries: In the first cell of the notebook, add the following code to install the required libraries
	`!pip install pandas==1.5.3 matplotlib==3.7.0 seaborn==0.12.2 scikit-learn==1.2.1`
	Run this cell by selecting it and clicking the "Run" button in Colab.
- Execute the Notebook: Change the path to hypotension_patients.csv if required and run each cell of the notebook sequentially by clicking the "Run" button or using the Shift+Enter keyboard shortcut.


## References and resources:
- Ahlqvist, E., Storm, P., Käräjämäki, A., Martinell, M., Dorkhan, M., Carlsson, A., Vikman, P., Prasad, R.B., Aly, D.M., Almgren, P. and Wessman, Y., 2018. Novel subgroups of adult-onset diabetes and their association with outcomes: a data-driven cluster analysis of six variables. The Lancet Diabetes & Endocrinology, 6(5), pp.361-369. [Clustering in medical field](https://pubmed.ncbi.nlm.nih.gov/29503172/)
- Roffman, C., Buchanan, J. and Allison, G., 2016. Charlson Comorbidities Index. Journal of Physiotherapy, 62(3).[Charlson Comorbidities Index](https://espace.curtin.edu.au/handle/20.500.11937/24203)
- Dataset outlier consultation - [Dr.J.Aman Kumar](https://www.practo.com/chennai/doctor/dr-j-aman-kumar-general-physician)

##Score
12.38/15 Points
