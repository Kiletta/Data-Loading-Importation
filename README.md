# Kajiado County Voter Statistics Analysis

Analysis of voter registration statistics in Kajiado County, Kenya, with a focus on Kajiado North Constituency. The notebook cleans, explores, and engineers features from raw voter data for demographic insight and machine learning applications.

# Data-Loading-Importation
This is a repository containing Data Loading in Data analysis for a wide range of  Datasets 

## Dataset

**Source:** `034 - 034.csv.csv`

**Key Columns:**
- Personal: `fname`, `mname`, `sname`, `id_passport_no`, `date_of_birth`
- Location: `county`, `constituency`, `county_assembly_ward`, `polling_center`, `polling_station`
- Demographics: `sex`, `age` (derived), `first_initial` (derived)

**Note:** Dataset contains personally identifiable information (PII). Handle appropriately and consider anonymization for public-facing analysis.

## Analysis Steps

1. **EDA** — Explore age/birth-year distribution, gender, geographic spread across CAWs and polling stations, and patterns specific to Kajiado North.
2. **Data Cleaning** — Handle missing values (fill `mname`, drop missing `fname`/`sname`), remove duplicates, optimize data types.
3. **Feature Engineering** — Create `full_name`, `name_length`, `age_group` bins, and retain `birth_year` explicitly.
4. **Encoding & Scaling** — One-hot encode categorical variables (`sex`, `age_group`); standardize numerical features (`age`, `name_length`).

## Output

Cleaned, type-optimized DataFrame with engineered features and scaled variables, ready for statistical analysis or ML modeling.

## Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
