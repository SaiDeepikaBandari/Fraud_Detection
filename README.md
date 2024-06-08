# Travelers Insurance Claim Fraud Detection

This project was part of a modelling competition- 2023 NESS Statathon.

Business problem:
You work for Travelers Insurance Company's fraud detection department as a modeler. Your colleagues, who are not familiar with statistics, would like you to create a predictive model based on historical claim data. Your team is concerned about the fraud detection accuracy as well as the key drivers that cause fraudulence.

Task is to identify first-party physical damage fraudulence and explain the indicators of fraudulent claims.

Data Overview:
Variable Descriptions

- claim_number - Claim ID (cannot be used in model)
- age_of_driver - Age of driver
- gender - Gender of driver
- marital_status - Marital status of driver
- safty_rating - Safety rating index of driver
- annual_income - Annual income of driver
- high_education_ind - Driver’s high education index
- address_change_ind - Whether or not the driver changed living address in past 1 year
- living_status - Driver’s living status, own or rent
- zip_code - Driver’s living address zipcode
- claim_date - Date of first notice of claim
- claim_day_of_week - Day of week of first notice of claim
- accident_site - Accident location, highway, parking lot or local
- past_num_of_claims - Number of claims the driver reported in past 5 years
- witness_present_ind - Witness indicator of the claim
- liab_prct - Liability percentage of the claim
- channel - The channel of purchasing policy
- policy_report_filed_ind - Policy report filed indicator
- claim_est_payout - Estimated claim payout
- age_of_vehicle - Age of first party vehicle
- vehicle_category - Category of first party vehicle
- vehicle_price - Price of first party vehicle
- vehicle_color - Color of first party vehicle
- vehicle_weight - Weight of first party vehicle
- fraud - Fraud indicator (0=no, 1=yes). This is the response variable.

# Data Cleaning ,EDA and Feature Engineering
 
 Performed Data Cleaning ,Exploratory Data Analysis and Feature Engineering to the data
 
- Mean/mode imputation for missing values
- Remove features that are clearly not useful e.g., vehicle_color,vehicle_weight
- Changed claim_date to a datetime variable  as it is a categorical variable to create more features
- Performed OneHotEncoding to Catrgorical data and Scaled Numerical Data
- Utilized SMOTE to handle class imbalance issues in the dataset

# Modeling

- Deployed Gradient Boosting to identify and flag fraudulent transactions in real-time, effectively minimizing false positives and false negatives, and significantly improving the reliability of real-time fraud identification processes and attained an F1 score of 0.91 through hyperparameter tuning.

  























