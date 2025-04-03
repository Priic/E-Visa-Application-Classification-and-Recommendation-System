# E-Visa-Application-Classification-and-Recommendation-System

![visa-application-approved_case](https://github.com/user-attachments/assets/70410323-ff35-4dbd-98eb-89be1a879e27)

## Context:

Business communities in the United States are facing high demand for human resources, but one of the constant challenges is identifying and attracting the right talent, which is perhaps the most important element in remaining competitive. Companies in the United States look for hard-working, talented, and qualified individuals both locally as well as abroad.
The **`Immigration and Nationality Act (INA)`** of the US permits foreign workers to come to the United States to work on either a temporary or permanent basis. The act also protects US workers against adverse impacts on their wages or working conditions by ensuring US employers' compliance with statutory requirements when they hire foreign workers to fill workforce shortages. 
**`The Office of Foreign Labor Certification (OFLC)`** processes job certification applications for employers seeking to bring foreign workers into the United States. Certifications are granted based on the unavailability of U.S. workers with the required skill set in a specific location.

With the **`increasing demand for visa applications `** each year, OFLC is seeking a **`Machine Learning-based solution`** to help shortlist candidates with a higher likelihood of visa approval. To address this challenge, they have `hired EasyVisa , consulting firm `to develop a data-driven approach for improving the decision-making process.
The `dataset` we have analyzed here consist of **`approx 26k visa applications details of the employees`**. They contains details  about **employees `educations, job experiences, continent`** of origin. Do they` require any job training` ? is the applications is for `full-time `or contract based position? details about `prevailing wages` and the units and `job locations` in USA . It aslo contains details about `employers company size(`i.e. number of employees ) and year it's established.

## Objective:

In FY 2016, the OFLC processed 775,979 employer applications for 1,699,957 positions for temporary and permanent labor certifications. This was a **nine percent increase** in the overall number of processed applications **from the previous year**. The process of reviewing every case is becoming a tedious task as the number of applicants is increasing every year.
The increasing number of applicants every year calls for a **Machine Learning based solution** that can help in shortlisting the candidates having higher chances of VISA approval. 
The main idea here is to analyze the data provided to **facilitate the process of visa approvals** and find which factors have a high influence in predicting the `visa application outcomes` and**`recommend`** a **`suitable profile`** for the applicants for whom the visa should be `certified or denied` based on these key drivers that significantly influence the case status.

## Model Building Approach:
As a Data Scientist,
1. **`Preprocessed`** data using **`Exploratory Data Analysis (EDA)`** and **`feature engineering`** to extract valuable insights and identify key features.
2. Developed multiple machine learning models `(Decision Tree, Bagging Classifier, Random Forest, AdaBoost, Gradient Boost, XGBoost, and Stacking)` to evaluate baseline performance before tuning.
3. Applied **`hyperparameter tuning using GridSearchCV`**, resulting in a significant `performance boost` (e.g., 6% increase in F1-score for Decision Tree) while reducing overfitting.
4. The model built helped in **`facilitate the process of visa approvals`** and **`recommend suitable applicant profiles`** for visa certification or denial and identify key factors influencing the decision.


## Data Description

The data contains the different attributes of the employee and the employer. The detailed data dictionary is given below.

* `case_id:` ID of each visa application
* `continent:` Information of continent the employee
* `education_of_employee:` Information of education of the employee
* `has_job_experience:` Does the employee has any job experience? Y= Yes; N = No
* `requires_job_training:` Does the employee require any job training? Y = Yes; N = No
* `no_of_employees:` Number of employees in the employer's company
* `yr_of_estab:` Year in which the employer's company was established
* `region_of_employment:` Information of foreign worker's intended region of employment in the US.
* `prevailing_wage:`  Average wage paid to similarly employed workers in a specific occupation in the area of intended employment. The purpose of the prevailing wage is to ensure that the foreign worker is not underpaid compared to other workers offering the same or similar service in the same area of employment.
* `unit_of_wage:`Unit of prevailing wage. Values include Hourly, Weekly, Monthly, and Yearly.
* `full_time_position:` Is the position of work full-time? Y = Full Time Position; N = Part Time Position
* `case_status:`  Flag indicating if the Visa was certified or denied
  
