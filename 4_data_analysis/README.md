# Data Analysis

[Non technical results of our war events data analysis here](https://github.com/MIT-Emerging-Talent/ET6-CDSP-group-03-repo/blob/non-technical-document/4_data_analysis/non_technical_results.md)

## 📘 Non-Technical Summary

We investigated how armed conflict affects students' academic performance and attendance, focusing
on the case of Gaza. Using data from public war events databases, we explored the impact of violence, displacement, infrastructure damage, and psychological trauma on online learning. Even
without full access to student performance records, our analysis highlights the deep, negative consequences of war on the learning environment.

Our findings reveal a direct correlation between periods of intense conflict and the deterioration of educational access and outcomes. High rates of civilian casualties, widespread destruction of
schools, and attacks on food supply chains have created severe conditions for students. These
hardships continue to affect their academic engagement.

[technical description of our war events data analysis here](https://github.com/MIT-Emerging-Talent/ET6-CDSP-group-03-repo/blob/main/4_data_analysis/technical_description.md)

## 🛠️ Technical Summary

Our team analyzed several war-related datasets to assess their impact on student life in Gaza, including casualties, displacement orders, infrastructure damage, and food supply disruption.
Each dataset was explored using simple rule-based logic, time-series analysis, and categorical aggregation depending on its structure.

We focused on extracting patterns by location, time, and type of impact. Data cleaning included standardizing dates, handling missing values, and filtering duplicates to ensure accuracy.

We deliberately avoided machine learning models due to the limited size and inconsistent structure of the data. Instead, we emphasized interpretability and correlation analysis—especially in areas like infrastructure and educational damage.

Each team member worked on a specific domain using Notebooks, and the combined results help us better understand how the war has affected access to education and students’ ability to learn under extreme conditions.

- [Casualities analysis](../3_data_exploration/casualties_data_analysis.ipynb)
- [Displasement orders analysis](../3_data_exploration/displacement_orders_EDA.ipynb)
- [Damage infrastructure analysis](../3_data_exploration/infrastracture_damaged_analysis.ipynb)
- [Food Supply Disruption analysis](../3_data_exploration/fivc_gaza_dataset_exploration_and_analysis.ipynb)
