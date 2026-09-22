# Loan Approval Data Analysis and Prediction System

## Project Overview

The **Loan Approval Data Analysis and Prediction System** is a Python-based data analysis project that explores historical loan application data to understand the factors associated with loan approval and rejection.

The project analyzes applicant information such as annual income, credit score, loan amount, years employed, and points. The data is prepared and analyzed using Python, and a simple predictive analysis technique is used to estimate the approval status of a new applicant.

The main focus of the project is **data analysis and interpretation**, with prediction used as an additional application of the analyzed data.

---

## Objectives

* Analyze historical loan application data.
* Understand the structure and characteristics of the dataset.
* Prepare relevant data for analysis.
* Analyze important applicant attributes.
* Examine approved and rejected loan applications.
* Identify patterns in the available data.
* Perform simple predictive analysis.
* Evaluate the prediction results.
* Generate an estimated loan approval result for a new applicant.

---

## Dataset

The project uses the **Loan Approval Dataset** available through Kaggle.

**Dataset Source:**
https://www.kaggle.com/

**KaggleHub Dataset Adapter Documentation:**
https://github.com/Kaggle/kagglehub/blob/main/README.md#kaggledatasetadapterpandas

The dataset used in this project contains:

* **2,000 records**
* **8 columns**
* No missing values in the supplied dataset

### Dataset Columns

| Column           | Description              | Usage    |
| ---------------- | ------------------------ | -------- |
| `name`           | Applicant's full name    | Not used |
| `city`           | Applicant's city         | Not used |
| `income`         | Annual income            | Used     |
| `credit_score`   | Credit score             | Used     |
| `loan_amount`    | Requested loan amount    | Used     |
| `years_employed` | Number of years employed | Used     |
| `points`         | Applicant points         | Used     |
| `loan_approved`  | Loan approval result     | Target   |

### Outcome Distribution

| Loan Status | Records |
| ----------- | ------: |
| Approved    |     879 |
| Rejected    |   1,121 |
| Total       |   2,000 |

---

## Technologies Used

### Programming Language

* Python

### Libraries

* **Pandas** – used for loading, handling, and preparing the dataset.
* **Scikit-learn** – used for dataset splitting, predictive analysis, and evaluation.

### Development Environment

* Google Colab
* Jupyter Notebook
* Visual Studio Code

---

## Project Workflow

The project follows a simple data analysis workflow:

```text
Dataset
   ↓
Load Data
   ↓
Understand Dataset
   ↓
Check Data Quality
   ↓
Select Relevant Attributes
   ↓
Prepare Data
   ↓
Analyze Applicant Data
   ↓
Perform Predictive Analysis
   ↓
Evaluate Results
   ↓
New Applicant Input
   ↓
Estimated Loan Result
```

---

## Features Used

The following attributes are used in the analysis and prediction process:

1. **Income**

   * Represents the applicant's annual income.

2. **Credit Score**

   * Represents the applicant's credit-related score.

3. **Loan Amount**

   * Represents the amount requested by the applicant.

4. **Years Employed**

   * Represents the applicant's employment duration.

5. **Points**

   * Represents the additional points value available in the dataset.

The `name` and `city` columns are not used because they are not required for the numerical analysis and prediction performed in this project.

---

## Prediction Technique

A simple **Logistic Regression** technique is used for the predictive analysis portion of the project.

The `loan_approved` column contains two outcomes:

```text
TRUE  →  1 → Loan Approved
FALSE →  0 → Loan Rejected
```

The dataset is divided into:

* **80% training data**
* **20% testing data**

The prediction results are evaluated using accuracy.

For the selected dataset split, the obtained accuracy was:

```text
1.0 (100%)
```

This result represents the performance on the particular test data used in the project and should not be interpreted as a guarantee of performance on new real-world loan applications.

---

## Installation

Make sure Python is installed on your system.

Install the required libraries using:

```bash
pip install pandas scikit-learn
```

### Optional: KaggleHub

If you want to access Kaggle datasets through KaggleHub, install:

```bash
pip install "kagglehub[pandas-datasets]"
```

KaggleHub documentation:

https://github.com/Kaggle/kagglehub/blob/main/README.md#kaggledatasetadapterpandas

---

## How to Run

### 1. Clone or download the project

Download the project files to your computer.

### 2. Place the dataset

Make sure `loan_approval.csv` is available in the project folder.

The folder should look like:

```text
Loan_Approval_Data_Analysis/
│
├── loan_approval.csv
├── loan_approval_prediction.py
├── requirements.txt
└── README.md
```

### 3. Install dependencies

Run:

```bash
pip install pandas scikit-learn
```

### 4. Run the Python program

```bash
python loan_approval_prediction.py
```

### 5. Enter applicant details

The program will ask for:

```text
Enter annual income:
Enter credit score:
Enter loan amount:
Enter years employed:
Enter points:
```

After entering the information, the program displays:

```text
Loan Approved
```

or

```text
Loan Rejected
```

---

## Google Colab

The project can also be executed using Google Colab.

Upload the `loan_approval.csv` file to the Colab environment and use:

```python
import pandas as pd

df = pd.read_csv("loan_approval.csv")
```

Then execute the remaining project code.

---

## Project Structure

```text
Loan_Approval_Data_Analysis/
│
├── loan_approval.csv
│       └── Dataset used for the project
│
├── loan_approval_prediction.py
│       └── Main Python program
│
├── requirements.txt
│       └── Required Python libraries
│
└── README.md
        └── Project documentation
```

---

## Key Data Analysis Points

The project provides the following analysis-related observations:

* The dataset contains 2,000 loan application records.
* Both approved and rejected applications are present.
* Rejected applications are higher than approved applications in the available dataset.
* Income, credit score, loan amount, employment duration, and points provide useful applicant information.
* These attributes can be studied to understand patterns associated with loan outcomes.
* Data preparation is an important step before performing predictive analysis.
* Historical application data can be used to support data-driven analysis and preliminary predictions.

---

## Future Enhancements

The project can be extended by adding:

* Data visualization using charts and graphs.
* Interactive dashboards.
* Detailed statistical analysis.
* Correlation analysis between numerical attributes.
* Distribution analysis of applicant information.
* Confusion matrix and additional evaluation metrics.
* Larger and more diverse datasets.
* A web-based interface for entering applicant information.
* More detailed explanations of prediction results.

---

## Disclaimer

This project is developed for **educational and internship purposes** to demonstrate data analysis and predictive analysis using a loan application dataset.

The prediction generated by the system should not be considered an actual financial or banking decision.

---

## Author

**Project:** Loan Approval Data Analysis and Prediction System

**Domain:** Data Analysis

**Language:** Python
