# 🎬 Feature Extraction of Anime Dataset

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Numpy](https://img.shields.io/badge/Numpy-Numerical%25Computing-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)](https://github.com/)

*An advanced data engineering and feature extraction pipeline transforming unstructured anime records into structured analytical metrics using Python and Pandas.*

---

## 📊 Professional Project Dashboard

| Module ID | Analytical Focus | Core Methodology & Scope | Difficulty | Status |
| :---: | :--- | :--- | :---: | :---: |
| **01** | **Dataset Ingestion & Profiling** | Structural validation, missing value audits, and schema verification of raw anime records. | Beginner | Completed ✅ |
| **02** | **Text Parsing & Cleaning** | Regular expression and string manipulation to isolate raw episode counts, date windows, and scores from compound attributes. | Intermediate | Completed ✅ |
| **03** | **Feature Engineering** | Mathematical computation of temporal durations (`Total_Months`) and standardized broadcast ranges. | Intermediate | Completed ✅ |

---

## 🧠 Comprehensive Module Breakdown

### 1. Dataset Ingestion & Profiling
* **Objective**: Ingest the raw CSV record base, check structural dimensions, and define data types.
* **Key Technical Takeaways**:
  * Successfully loaded raw records using optimized Pandas `read_csv` routines.
  * Evaluated feature dimensions and initial data hygiene to detect irregularities.
  * Identified unstructured compound strings residing in core columns that require parsing.

### 2. Text Parsing & Cleaning
* **Objective**: Isolate discrete structural elements from mixed, unparsed string attributes.
* **Key Technical Takeaways**:
  * Applied string slicing and pattern-matching techniques to separate title names, broadcast statuses, and metadata.
  * Extracted numerical episode values and cast them into clean integer fields.
  * Cleaned and standardized start/end broadcast date strings for downstream calculations.

### 3. Feature Engineering
* **Objective**: Transform isolated datetime markers into quantitative analytical features.
* **Key Technical Takeaways**:
  * Parsed start and end month-year indicators using Python's `datetime.strptime` module.
  * Engineered the `Total_Months` metric via custom delta equations (`(end_year - start_year) * 12 + (end_month - start_month) + 1`).
  * Validated calculations across multi-year runs and seasonal distributions.

---

## 💻 Core Implementation Snippet

```python
from datetime import datetime
import pandas as pd

# Load and process dataset
df = pd.read_csv('anime.csv')

def calculate_total_months(time_str):
    parts = time_str.split(' - ')
    start_date = datetime.strptime(parts[0], "%b %Y")
    end_date = datetime.strptime(parts[1], "%b %Y")
    
    total_months = (end_date.year - start_date.year) * 12 + (end_date.month - start_date.month) + 1
    return total_months

df['Total_Months'] = df['Total Time'].apply(calculate_total_months)
