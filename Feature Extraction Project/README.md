# 🎬 Feature Extraction of Anime Dataset: Pipeline & Analysis

`PYTHON 3.10+` `PANDAS` `DATA ANALYSIS` `NUMPY` `NUMERICAL COMPUTING` `STATUS COMPLETED`

*An advanced data engineering and feature extraction pipeline transforming unstructured anime records into structured analytical metrics using Python and Pandas.*

---

## 📊 Professional Project Dashboard

| Module ID | Analytical Focus | Core Methodology & Scope | Difficulty | Status |
| :---: | :--- | :--- | :---: | :---: |
| **01** | **Dataset Ingestion & Profiling** | Structural validation, missing value audits, and schema verification of raw anime records. | Beginner | Completed ✅ |
| **02** | **Text Parsing & Cleaning** | Regular expression and string manipulation to isolate raw episode counts, date windows, and scores from compound attributes. | Intermediate | Completed ✅ |
| **03** | **Feature Engineering** | Mathematical computation of temporal durations (`Total_Months`) and standardized broadcast ranges. | Intermediate | Completed ✅ |
| **04** | **Pipeline Export & Validation** | Final integrity checks, schema mapping, and exporting the structured dataset (`anime_processed.csv`). | Advanced | Completed ✅ |

---

## 🧠 Comprehensive Module Breakdown

### 1. Dataset Ingestion & Profiling ( `ingest.py` )
* **Objective**: Ingest the raw CSV record base, check structural dimensions, and define data types.
* **Key Technical Takeaways**:
  * Successfully loaded raw records using optimized Pandas `read_csv` routines.
  * Evaluated feature dimensions and initial data hygiene to detect irregularities.
  * Identified unstructured compound strings residing in core columns that require parsing.

### 2. Text Parsing & Cleaning ( `parser.py` )
* **Objective**: Isolate discrete structural elements from mixed, unparsed string attributes.
* **Key Technical Takeaways**:
  * Applied string slicing and pattern-matching techniques to separate title names, broadcast statuses, and metadata.
  * Extracted numerical episode values and cast them into clean integer fields.
  * Cleaned and standardized start/end broadcast date strings for downstream calculations.

### 3. Feature Engineering ( `features.py` )
* **Objective**: Transform isolated datetime markers into quantitative analytical features.
* **Key Technical Takeaways**:
  * Parsed start and end month-year indicators using Python's `datetime.strptime` module.
  * Engineered the `Total_Months` metric via custom delta equations (`(end_year - start_year) * 12 + (end_month - start_month) + 1`).
  * Validated calculations across multi-year runs and seasonal distributions.

### 4. Pipeline Export & Validation ( `pipeline.py` )
* **Objective**: Finalize the dataset structure, perform quality assurance checks, and export the output.
* **Key Technical Takeaways**:
  * Executed automated assertions to verify data integrity across all engineered columns.
  * Exported clean, analysis-ready tabular data to `anime_processed.csv`.
  * Packaged core transformation functions into a modular, reusable script architecture.

---

