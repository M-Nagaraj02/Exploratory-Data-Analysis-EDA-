# 📊 Exploratory Data Analysis (EDA) Using Pandas & NumPy
---
## Overview

This project demonstrates Exploratory Data Analysis (EDA) using Pandas and NumPy.
The dataset contains cricket players' details such as Practice Hours, Matches Played, and Runs Scored.

The goal of this project is to:

* Clean the data
* Handle missing values
* Convert data types
* Detect and treat outliers
* Prepare structured data for further analysis

---
## Dataset

The dataset is manually created using a Python dictionary.
Features included:

* ID
* Name
* Teams
* Practice_Hours
* Gender
* Playing_Match
* Runs
```python
import pandas as pd
import numpy as np
```
* Total Records: 10
* Total Columns: 7

## Methodology
**1️⃣ DataFrame Creation**
* Converted dictionary into Pandas DataFrame

**2️⃣ Data Type Conversion**
* Converted numerical columns from object → numeric

Used ``` pd.to_numeric()```

**3️⃣ Handling Text Errors**

* Replaced:

  * "Fourteen" → NaN
  * "Unavailable" → NaN

**4️⃣ Missing Value Detection**

* Used:
 ```python 
   isna().sum()
   isnull().sum()
```
**5️⃣ Handling Missing Values**

* Filled missing IDs with 104
* Filled missing Playing_Match with 10
* Filled missing Runs using mean value
* Treated outlier in Practice_Hours (100 → replaced with mean)
 
**6️⃣ Outlier Treatment**

* Detected abnormal value (Practice_Hours = 100)
* Replaced with NaN
* Filled with mean value
---

## Key Operations Used

``` python
pd.DataFrame()
pd.to_numeric()
.replace()
.fillna()
.isnull()
.mean()
.loc[]
```
---

## Results

* Successfully cleaned inconsistent data
* Converted all numeric columns to proper data types
* Handled missing values properly
* Treated outliers effectively
* Final dataset ready for further analysis or modeling

---
## Final Cleaned Dataset

**The dataset after cleaning:**
* No missing values
* Correct data types
* Outliers handled
* Structured and analysis-ready

---
## Project Structure

EDA-Project/
* │── EDA_Notebook.ipynb
* │── README.md
---
## Skills Demonstrated

* Data Cleaning
* Data Preprocessing
* Handling Missing Values
* Outlier Detection
* Pandas Data Manipulation
* Exploratory Data Analysis

---
## Author

**Nagaraj M**

GitHub: https://github.com/M-Nagaraj02
