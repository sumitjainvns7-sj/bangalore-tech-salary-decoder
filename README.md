# Bangalore Tech Salary Decoder 🐼💼

An end-to-end Python and Pandas data cleaning, manipulation, and analytics project built during **The Unlox Academy 2-Hour Live Project Sprint**[cite: 4, 5]. This tool parses, normalizes, and decodes a messy dataset of over 1,015 technology professionals in Bengaluru to uncover key structural patterns in tech compensation[cite: 25].

## 🚀 Project Overview
In real-world scenarios, HR and compensation data is intentionally messy, fragmented, and non-standardized[cite: 26]. This project implements a full analytical pipeline that ingests raw, dirty data, executes robust cleaning algorithms without using restrictive regex elements, runs targeted business intelligence queries, and renders a production-ready ASCII executive dashboard[cite: 59, 65, 99].

## 🛠️ Key Features & Technical Workflow

### 1. Data Quality Inspection (Task 1)
* Analyzed initial structural footprints using `info()`, `shape`, and missing value sums[cite: 59].
* Identified mixed data types, duplicate entries, and mapped data deficits (e.g., isolating 200 missing values in previous salary tracking).

### 2. Algorithmic Data Cleaning & Normalization (Task 2)
* **Column Standardization:** Transformed messy headers into uniform, clean `snake_case` column configurations[cite: 65].
* **Robust Salary Parsing:** Engineered custom parsing logic to translate 4 distinct string formats—including absolute values like `15,50,000` and text suffixes like `15.5 LPA`—into clean, uniform floating-point numbers in LPA units[cite: 33, 34, 68].
* **Categorical Unification:** Standardized role variants (e.g., mapping `ds` and `data scientist` uniformly) along with company types and education tier labels[cite: 29, 37, 41, 66].

### 3. Core Business Intelligence Queries (Task 3)
* **Q3.1 Role Distributions:** Evaluated compensation metrics (median, mean, minimum, maximum) across all primary domains, sorting by high-water baselines[cite: 80].
* **Q3.2 Experience Curves:** Binned continuous engineering experience into 4 discrete buckets (`0-1`, `2-3`, `4-5`, `6+`) using `pd.cut()` to inspect career compounding trends[cite: 82, 83].
* **Q3.3 Skill Premiums:** Isolated exact salary deltas via targeted vector string tracking (`.str.contains()`) to find the financial impact of specialized technical tools[cite: 85, 86].
* **Q3.4 Company Premiums:** Calculated cross-organizational variance between venture-backed scales and traditional corporate structures[cite: 88, 89].
* **Q3.5 Underpaid Anomalies:** Combined `groupby`, `transform`, and conditional filtering to compute cohort medians and isolate individual professionals sitting furthest below their baseline market groups[cite: 90, 91, 93].

## 📊 Live Report Architecture (Task 4)
The pipeline features an automatic dashboard built with pure Python string width specifiers, alignment systems, and custom dividers to format absolute trends cleanly[cite: 99]:
* **Proportional ASCII Bar Charts** indicating median packages across domains.
* **Sequential Career Curves** highlighting experience-tier compounding margins.
* **Stratified Premium Matrixes** for infrastructure tools and structural employer variance.
* **Anomalous Gap Isolation** outlining individual underpaid profiles.

## 🐍 Tech Stack
* **Language:** Python 3.12
* **Core Libraries:** Pandas, NumPy
* **Environment:** Jupyter Notebook / Google Colab [cite: 19, 280]

---
*Built with passion as part of the Unlox Academy Industry Sprint.* 🚀
