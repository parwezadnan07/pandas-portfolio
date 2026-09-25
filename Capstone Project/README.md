<div align="center">

# 🌐 Global Countries Dataset: Exploratory Data Analysis & Dashboard

<p align="center">
  <img src="https://img.shields.io/badge/PYTHON-3.10%2B-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/PANDAS-DATA_ANALYSIS-darkgreen.svg" alt="Pandas">
  <img src="https://img.shields.io/badge/NUMPY-NUMERICAL_COMPUTING-orange.svg" alt="NumPy">
  <img src="https://img.shields.io/badge/STATUS-COMPLETED-brightgreen.svg" alt="Status">
</p>

*An enterprise-grade analytical repository exploring global geographical, demographic, economic, and political indicators using Python and Pandas.*

</div>

---

## 📊 Professional Project Dashboard

| Module ID | Analytical Focus | Core Methodology & Scope | Difficulty | Status |
| :---: | :--- | :--- | :---: | :---: |
| **01** | **Dataset Overview** | Structural profiling, dimensionality checks, and feature categorization (194 entities, 64 columns). | Intermediate | Completed ✅ |
| **02** | **Demographics & Geography** | Population extrema tracking, capital identification, and microstate analysis. | Intermediate | Completed ✅ |
| **03** | **Governance & Democracy** | Democracy index scoring, political leadership auditing, and naming nomenclature patterns. | Advanced | Completed ✅ |
| **04** | **Regional Clustering** | Macro-region classification (22 regions) and Eastern Europe cluster isolation (10 nations). | Advanced | Completed ✅ |

---

## 🧠 Comprehensive Module Breakdown

### 1. Dataset Structural Profiling ( `analysis.py` )

* **Objective:** Audit and categorize the raw global indicators dataset to understand its structural composition and data types.
* **Key Technical Takeaways:**
  * Successfully ingested and verified a dataset comprising **194 sovereign entities and territories**[cite: 5].
  * Evaluated feature dimensionality totaling **64 distinct columns**[cite: 5].
  * Systematically categorized features into **48 float attributes, 6 integer attributes, and 10 string/text attributes**[cite: 5].

---

### 2. Demographic & Geographic Extremes ( `population_metrics.py` )

* **Objective:** Extract and analyze population distributions, extremes, and capital city mappings across global entities.
* **Key Technical Takeaways:**
  * Identified **India** (with New Delhi as its capital) as the most populous entity, followed by China as the second largest[cite: 5].
  * Isolated microstates like **Tuvalu** (with Funafuti as its capital) as recording the lowest population thresholds in the dataset[cite: 5].
  * Mapped global entities across **22 distinct geographic regions**[cite: 5].

---

### 3. Governance & Political Structures ( `governance_audit.py` )

* **Objective:** Analyze political regime types, democracy index rankings, state nomenclature, and leadership data completeness.
* **Key Technical Takeaways:**
  * Pinpointed top-tier democratic nations boasting the highest democracy scores, led by **Norway, Iceland, Sweden, New Zealand, and Denmark**[cite: 5].
  * Audited state nomenclature patterns, discovering that exactly **125 countries** incorporate the term "Republic" within their official long-form names[cite: 5].
  * Flagged data quality gaps by identifying **7 countries** with unrecorded or missing political leadership records[cite: 5].

---

### 4. Regional Clustering & Eastern Europe ( `regional_analysis.py` )

* **Objective:** Isolate specific macro-regional groupings to perform localized comparative analysis.
* **Key Technical Takeaways:**
  * Extracted and examined the **Eastern Europe** cluster consisting of **10 core nations**[cite: 5].
  * Cataloged cluster members including Russia, Ukraine, Poland, Romania, Czech Republic, Hungary, Bulgaria, Slovak Republic, Moldova, and Belarus[cite: 5].

---

## 🛠️ Tech Stack & Requirements
* **Language:** Python[cite: 5]
* **Data Manipulation & Compute:** Pandas, NumPy[cite: 5]
* **Environment:** Jupyter Notebook / Python 3.10+ Scripting Interface

---

## 🚀 Getting Started & Replication

To run the exploratory analysis script locally:

Install required dependencies:
pip install pandas numpy

Execute the analysis script:
python analysis.py



1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/countries-dataset-eda.git](https://github.com/your-username/countries-dataset-eda.git)
   cd countries-dataset-eda
