![Pulse Check Cover Photo](https://github.com/user-attachments/assets/ec160890-7692-493d-87cb-9eb0294ac7e6)

# Pulse Check: Tapping into Diabetes Care Across 130 US Hospitals 

## Project Background
This analysis examines ten years (1999-2008) of clinical care data from 130 US hospitals, focusing on diabetes patient care patterns and resource utilization. The project explores how different departments handle diabetic patients, analyzing variations in care delivery and hospital resource allocation across different patient groups and medical specialties.

Insights and recommendations are provided on the following key areas:

* **Racial Equity in Care**: An assessment of lab procedures and if there is a significant difference in treatment between races
* **Hospital Resource Utilization**: Analysis of lab procedure volume by department to determine which are most resource intensive
* **Emergency Care Efficiency**: Evaluating the triage efficiency of emergency care by comparing average days in hospital
* **Length of Stay Analysis**: Examining the overall length of stay of patients

* Targeted SQL queries regarding various operation quests can be found [here](https://docs.google.com/document/d/1W5pK3_eNoK_2_T-1awVWICYyTHJ87eXtzlc4m5aI3hw/edit?tab=t.0)
* Original data set can be found  [here](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)

## Data Structure & Initial Checks

Dataset Characteristics:
- 101,766 patient records
- 47 features per record
- Mix of categorical and integer data types
- Contains sensitive demographic information
- Includes missing values

The dataset comprises over 47 features including:

Patient Metrics:
- Demographics (race, gender, age)
- Admission type
- Length of stay
- Previous visit history (outpatient, inpatient, emergency

Inclusion Criteria:
1. Inpatient hospital admissions only
2. Confirmed diabetes diagnosis
3. Length of stay: 1-14 days
4. Includes laboratory tests
5. Includes medication administration

Clinical Information:
- Medical specialty of admitting physician
- Laboratory test counts and results
- HbA1c test results
- Medication details
- Diabetic-specific treatments

![ERD](https://github.com/user-attachments/assets/04ee4999-bed2-4d76-9207-b220ac585d08)


## Executive Summary

### Overview of Findings
Analysis of over 100,000 diabetic patient records reveals patterns in care delivery and resource utilization. While racial disparities in procedure counts are minimal, we identified significant variations across medical specialties. Emergency admissions show efficient processing, and length of stay patterns provide insights into hospital resource allocation.

## Insights Deep Dive

### Category 1: Racial Equity in Care
![race_lab_meds_time](https://github.com/user-attachments/assets/b65c9424-5fea-4fcf-9e0d-ad2f818448bf)
- Average lab procedure variations across racial groups are minimal, with maximum difference of four visits between African American and Asian patients
- Demographic analysis shows no significant systematic bias in care delivery
- Regular monitoring recommended to maintain care equity
  

### Category 2: Hospital Resource Utilization
![image](https://github.com/user-attachments/assets/e9cfc7db-7842-4b92-9203-cb345a76bb09)
- Cardiology specialties show highest procedure counts (>2.5 average procedures)

![image](https://github.com/user-attachments/assets/0dece43c-f590-4ce6-a037-6b04e9f1cb5a)
- Direct correlation between lab procedure quantity and hospital stay duration

### Category 3: Emergency Care Efficiency
![image](https://github.com/user-attachments/assets/b79c2fbe-0b90-4dd8-aaad-008e0f02593b)
- Emergency admissions average 4.378 days (below overall 4.395 day average)
- Non-emergency stays average 4.416 days
- Efficient emergency protocols demonstrate effective triage

### Category 4: Length of Stay Analysis
![image](https://github.com/user-attachments/assets/69563f97-7756-4212-8cca-237deeec8c0d)
- 79% of patients stay 1-6 days
- 21% remain 7+ days
- Equal acute/non-acute distribution across stay durations
- Longer stays correlate with increased procedure counts

## Recommendations

Based on our analysis, I recommend:

1. Maintain current equity in care delivery while continuing regular monitoring across demographic groups.

2. Consider resource allocation optimization for cardiology departments given their consistently higher procedure counts.

3. Study emergency care protocols for potential best practices that could be applied to other departments.

4. Develop specific care protocols for patients staying 7+ days, as they represent a significant resource-intensive population.

5. Implement automated tracking of procedure counts and length of stay correlations to identify resource optimization opportunities.

## Assumptions and Caveats

Important considerations and future directions:

1. Missing values in the dataset required careful handling and may impact certain metric (race, weight, 

2. The 14-day maximum stay criterion may exclude some complex cases.

3. Diabetes diagnoses are assumed to be accurately recorded across all facilities.

4. Historical data (1999-2008) may not fully reflect current medical practices in 2025.

5. Future Analysis Opportunities:
   - The dataset contains rich information about patient readmission patterns that could be analyzed in future studies
   - Additional investigation could explore relationships between care patterns identified in this study and patient outcomes
   - Potential analysis of how procedure counts and length of stay correlate with readmission rates


