# Technical Summary

## Why did we choose these algorithms?

Our team selected analytical strategies based on the structure and content of each dataset.  
Each participant chose methods best suited to their dataset’s format:

- **For casualties**: time-series trend analysis and categorical aggregation (e.g., by gender/age) helped reveal patterns in civilian impact.
- **For displacement orders**: chronological ordering and geographic tagging were key to understanding movement dynamics.
- **For infrastructure and food supply damage**: we applied damage categorization and impact scoring using rule-based logic. In addition, we performed correlation testing on the infrastructure damage dataset. This allowed us to explore relationships
between variables such as location,
facility type, and reported damage level.

## How did we account for quirks in the data?

Each dataset had specific challenges:

- Missing or inconsistent values were cleaned via imputation, removal, or standardization (e.g., replacing empty strings with `"unknown"`).
- Unstructured text fields (especially in infrastructure or displacement notes) were handled using keyword matching or regular expressions.
- Duplicate entries were filtered by unique identifiers and timestamps.
- Date formatting inconsistencies were normalized to ISO-8601 to enable accurate time-based analysis.

## What strategies/algorithms didn’t we use and why?

In particular, we avoided:

- Machine learning models (like random forests or deep learning), because the available data wasn’t large or structured enough to train such models effectively.
- Time-based predictive modeling, since we were analyzing past events rather than trying to forecast future outcomes.

---

## Individual Notebooks Overview

### Wour — Casualties Analysis

- **Focus**: Civilian casualty records (by age, gender, cause of death).
- **Method**: Aggregated and visualized casualties by demographic, location, and time.

### Salem — Displacement Orders Analysis

- **Focus**: Tracking evacuation and displacement notices.
- **Method**: Extracted location and time info, then created sequences of displacement events.

### Viktoriya — Infrastructure Damage Analysis

- **Focus**: Damaged churches, civil buildings, schools, etc.
- **Method**: Grouped by infrastructure type and region, calculated frequency and severity.

### Raneem — FIVC: Food Supply Disruption

- **Focus**: Damage to agricultural lands, bakeries, markets, and food infrastructure across regions.
- **Method**: Grouped by infrastructure type and region.

---

## Jupyter Notebooks

- [Wour](../3_data_exploration/casualties_data_analysis.ipynb)
- [Salem](../3_data_exploration/displacement_orders_EDA.ipynb)
- [Viktoriya](../3_data_exploration/infrastracture_damaged_analysis.ipynb)
- [Raneem](../3_data_exploration/fivc_gaza_dataset_exploration_and_analysis.ipynb)
