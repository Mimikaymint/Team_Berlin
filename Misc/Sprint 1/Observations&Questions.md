# Ticket 1.1.4: Initial Observations & Questions

## 1. Key Observations
- The dataset contains multiple CSV files: 
  - `training_set_features.csv`
  - `training_set_labels.csv`
  - `test_set_features.csv`
  - `submission_format.csv`
- Dataset profile summary is available in `Team Berlin/Misc` folder.
- Features include both numerical(labelled data) and categorical variables.
- There are missing values in some columns that will need handling.
- The missing values in columns(employmemt_industry, occupation and health_insurance) are  more than 50% and will be investigated further before deletion.
- The data structure suggests a supervised learning task (predicting labels from features).
- Notebook organization: all files are currently located in `Team Berlin folder` folder.
- For target variables, seasonal vaccines were taken more than the h1n1 vaccines.

## 2. Potential Challenges
- Missing data may require imputation or careful preprocessing.
- Some features may need encoding (e.g., categorical variables) for machine learning models.
- Class imbalance in labels could affect model performance.
- Large dataset may lead to longer computation times.
- Confusion regarding relative paths and folder structure has caused errors in data loading.

## 3. Research Questions
- Which features are the most significant predictors of whether an individual receives a flu shot?
- How do demographics such as the Age group, Sex snd income etc influence the reception of the flu shot?.
- How do behavioural pattens influence the reception of the flu shot?.
- Are there distinct groups of individuals (clusters) with similar characteristics in relation to flu shot behaviour, and what are their profiles?
- How do personal beliefs and opinions (e.g., opinion_h1n1_vacc_effective, opinion_seas_risk) influence the likelihood of receiving H1N1 or seasonal flu vaccines?

## 4. Questions for Further Investigation
- Which features are most predictive of the target labels?
- Are there correlations between features that may affect model performance?
- How to handle missing values in a way that minimizes bias?
- Should we normalize/scale numerical features for modeling?
- What evaluation metrics are most suitable for this dataset?
- Are there any anomalies or outliers that need to be addressed?
- How can we organize folders and files for easier reproducibility?


