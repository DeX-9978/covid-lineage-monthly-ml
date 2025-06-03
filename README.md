# COVID-19 Lineage Classification (Malaysia, June 2021–Jan 2022)

This project uses Malaysian SARS-CoV-2 molecular epidemiology data to predict the most prevalent variant (lineage) in a given month using machine learning.

## Objective
Classify the most dominant SARS-CoV-2 lineage based on lineage prevalence percentages in a given month.

## Data
- Extracted from Supplementary Table 2 of this study --> (https://www.ijidonline.com/article/S1201-9712(22)00582-3/fulltext)
- 8 rows (June 2021 to January 2022), 10 lineage features

## Methods
- Data cleaning using regex to extract percentages
- Feature engineering to determine most prevalent lineage
- Random Forest classifier
- Evaluation via classification report and 3-fold cross-validation

## Results
- Accuracy (cross-validation): ~50%
- Best model: RandomForestClassifier (default settings)

## Limitations
- Very small dataset (8 rows)
- Only monthly summary used (no spatial features)
- Model performance is not reliable due to small sample size

## Next Steps
- Expand dataset using state-wise lineage prevalence
- Add time-series modeling or mutation-level analysis
