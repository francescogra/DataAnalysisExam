# Data Analysis Exam Project - University of Catania

## Project Title
**Cardiovascular Study Dataset - Predicting Heart Disease of Patients**

## Project Overview
This repository contains the exam project for the Data Science course on Data Analysis at the University of Catania. 
<p>This repository has only eductional purposes, so it is freely usable (just put the link of this repository as a reference in your README file if you do).</p>

## What is it about?

<p>I won't go further with the explanations since I have explained more in the notebook.</p>

<p>Anyway, the goal of this project is to study a dataset with a various number of data science tools. The dataset I've picked is about cardiovascular diseases. We want to retrieve meaningful information from it and eventually be able to use this data for specific operations (such as classification, clustering, regression etc.).</p>

<p>More details about how I retrieved the data, what are the system requirements and so on will be explained in-depth in the notebook</p>

## How to run

<p>I suggest using CONDA to manage the python environments. You can easily set up a new CONDA env and delete it once you don't need it anymore.</p>

<p>To install CONDA you can check this <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html#">website</a>.</p>

<p>This is the code to run in your shell once you have Conda to create the envinroment with the needed packages to run notebooks:</p>

```bash
conda create -n fad python=3.8
conda activate fad
conda install -c anaconda jupyter
```

<p>This is the code to run in your shell to run jupyter notebooks:</p>

```bash
cd <repository-folder>/
jupyter notebook
```

## How to remove the environment

<p>This is the code to run if you want to delete the environment:</p>

```bash
conda deactivate
conda env remove -n fad
```

# 🧑‍💻 Accessing the File
This project's notebook is saved as an .ipynb file. Here are a few options for accessing it:

1.  Upload to Jupyter Notebook:
    If you have Jupyter Notebook installed, open it in your browser.
    Upload the .ipynb file by clicking on “Upload” on the main page, then navigating to the project file.
    Once uploaded, click on the file to open it and start running each cell.

2.  Running on Google Colab:
    You can also run this notebook on Google Colab. Go to Google Colab, select “Upload notebook,” and upload the .ipynb file.
    Colab allows you to run the code directly in the cloud, without having to install local libraries.
    Opening in VS Code:

3.  Visual Studio Code, with the Jupyter extension installed, can execute .ipynb files.
    Open VS Code, select "File" > "Open File," navigate to the .ipynb file, and open it. VS Code will allow you to run the code in a notebook format.


# Project Dependencies
To run the notebook and reproduce the analysis, you'll need to install the following modules:

1.    numpy
2.    pandas
3.    matplotlib
4.    scipy
5.    seaborn
6.    statsmodels
7.    imbalanced-learn

# Purposes
World Health Organization has estimated 12 million deaths occur worldwide, every year due to Heart diseases. Half the deaths in the United States and other developed countries are due to cardio vascular diseases. The early prognosis of cardiovascular diseases can aid in making decisions on lifestyle changes in high risk patients and in turn reduce the complications.

This notebook main purpose was to study one of the many Framingham Heart Diseases datasets. The research on this dataset was organized in these three main sections:

Section one: Data Analysis and Data Refactor (Chapter 3)
Section two: Descriptive statistics on the data (Chapter 4)
Section three: Classification (Chapter 5)


#  About the dataset
The dataset is publically available on the Kaggle website. It contains the data of over 4000 residents of the town of Framingham, Massachusetts. The meaning of this dataset is to determine if the patients will suffer at least a CHD (coronary heart disease) or not in ten years.

To be able to reach this goal, for each person there are fifteen attributes divided in three groups: demographic, medical history of the patient and his or her current medical status (such as BMI, heart rate etc). Each attribute is a potential risk factor to determine if the patient will suffer a CHD in ten years.

Here the list of the attributes:

Demographic
sex: male (value 1) or female (value 0)
age: Number of years as an integer number
education: Some High School (value 1); High School Degree or GED (value 2); Some College or Vocational School (value 3); College Degree or Vocational School Degree (value4)
currentSmoker: Smoker (1) or Nonsmoker (0)
cigsPerDay: Average number of cigarettes smoked per day as an integer (0 for nonsmokers)
Medical History of the patient
BPMeds: Whether the patient is on Blood Pressure medications (value 1) or not (value 0)
prevalentStroke: Whether the patient already had at least a stroke (value 1) or not (value 0)
prevalentHyp: Whether the patient is hypertensive (value 1) or not (value 0)
diabetes: Whether the patient has diabetes (value 1) or not (value 0)
Current Medical Status of the patient
totChol: Float number of the cholesterol measured as mg/dL
sysBP: Float number of the systolic blood pressure measured as mmHg
diaBP: Float number of the diastolic blood pressure measured as mmHg
BMI: Body Mass Index (weight/height
) of the patient measured as kg/mt
. It is a float number
heartRate: Beats/Minute. It is an integer number
glucose: Float number of the quantity of glucose in the patient's blood. Measured as mg/dL
As we said, this dataset is labeled. The column's name is TenYearCHD. There are two classes:

Class 0: The patient won't have a CHD disease in 10 years.
Class 1: The patient will have at laest one CHD disease in 10 years.
