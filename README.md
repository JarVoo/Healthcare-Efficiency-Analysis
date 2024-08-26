# Healthcare Analysis with Power BI

### Dashboard Link : https://app.powerbi.com/groups/me/reports/384e33e8-b9b8-4ed7-99be-dae870f0f268/0367c202c2f375fe20a5?experience=power-bi


![home page](https://github.com/user-attachments/assets/e6c78143-4ea9-4536-a0ef-a4e22be7c51f)

 


## Introduction

In the healthcare industry, one of the frameworks for healthcare quality is efficiency among many others. In this analysis, efficiency is the main focus, and within the domain, Length of Stay (LOS) is used to measure efficiency in hospital management. 

All hosipitals want shorter LOS, as costs are lowered, it releases capacity in the system, allowing more patients to be attended to.This case study looks specifically at Elective Hip Replacement procedures using New York state-wide hospital data over a 1 year period.

## Problem Statement


A hospital recovery stay should be anywhere from 0-2 days but can be extended for various reasons. I will dig deep and find out what these reasons are that some hospitals have longer LOS days.I will also look into the cost to the hospitals for these extra days needed in a care facility.

- Which Hospitals stand out with the highest cost compared to the state average.
- Which Hospitals stand out as the biggest outliers
- Root Cause Analysis: What factors influence LOS and cost the most?


Some important domain vocabulary to understand the analysis:

- Length of Stay: Total days the patient stayed in hospital, including surgery, and recovery time.
- Patient disposition: patients destination after discharge.
- Elective surgery: procedures that were planned in advance, not due to an emergency.
- Total Cost: Total cost for the stay and any procedures done.



### Data Collection and Understanding

The data was collected from 151 hospitals within the New York state over a 1 year period by a consulting company called HealthStat. They captured patient-level data on all hospital stays. My first task was to import the data into Power BI and profile the data for anything strange:

    1) Surgical prodecures that didnt include elective hip replacement were filtered out. 
    2) I performed EDA about the patient and hospital data which revealed that there were 151 hospitals with New York City housing most of the hospitals.

![Total Hospitals](https://github.com/user-attachments/assets/5e564f8b-81ac-406a-8928-f0827cab4845)

    3) In the patient data, there were 26,286 discharges in the year with 53.7% female and 46.3% male. Hip replacement procedures were mostly conducted on the 50 and older age groups.

![Patient Profile](https://github.com/user-attachments/assets/0bd8467f-c8f3-48b3-b116-915b0ef5fee6)

    4) Various metrics were calculated such as:
        - average LOS days,
        - total surgeons,
        - average cost per discharge 

### Exploratory Data Analysis

Using the efficiency metric, Length of Stay (LOS) days with other demographic fields, it was interesting to find that, on average, Males aged 50 or older stayed in hospital an average of 2,53 days for their hip replacement procedure.   

The leadership team wanted some visibility on how average LOS days and total discharges compare between hospitals:

![LOS Comparison](https://github.com/user-attachments/assets/b58f8e6b-f093-4da7-a24d-b2ac83efeefa)

Syosset hospital was the highest average LOS days (3.22) and there were 11 surgeons that conducted Elective Hip Surgery that year. Hospital for Special Surgery had the highest number of discharges.

Kings County Hospital Centre in New York City had an average LOS of 12 days with a whopping 352.59%  higher than the state average

 - Next I wanted to know why some hospitals have much longer LOS days than others.


![Cost Comparison](https://github.com/user-attachments/assets/4bae77f6-7a9f-44dc-b2aa-cc70f8335a11)
The average cost per discharge for the state is $20,910. 
.

From a root cause analysis, the top influencers increased average LOS days and cost:

    1) Extreme illness severity
    2) Extreme/Major mortality risk
    3) Hospitals in New York City
    4) Patient disposition to skilled nursing homes.




 


# Insights


The Following inferences can be drawn from the dashboard;

### [1] Total Number of Discharges = 26,286

   Average Cost per Discharge = $20,910

   Hospital with the most and least discharges:

   - Hospital for Special Surgery (4,515)
   - Millard Filmore Suburban Hospital (414)

   Highest average cost per discharge Key influencers:

   - Patient disposition = Inpatient Rehabilitation Facility
   - Risk of mortality = Extreme
   - Severity of illness = Extreme
           
### [2] LOS Days

Average LOS days = 2.65

Top 3 hospitals with highest LOS:

    1) Kings County Hospital Centre (12 days)
    2) Interfaith Medical Centre (9.33 days)
    3) Memorial Hospital for Cancer and Allied Diseases (9.1 days)


The most efficient hospitals included:

    1) Northern Dutchess Hotel (1.37)
    2) St Elizabeth Medical Centre (1.56 days)
    3) Alice Hyde Medical Centre (1.68 days)

## Conclusions

LOS days are correlated with average cost per discharge. The hospitals that were identified to have long period LOS had a high cost and deemed inefficient. While hospitals with low LOS days and low cost were deemed efficient. It is difficult however to make this a very clear assumption without diving into a deeper root cause analysis. 

For example, hospitals with high LOS days and High average cost, could also suggest other factors, such as care intensity or hospital inefficiencies, which could also be driving higher costs. However streamlining processes, improving care coordination and reducing complications to improve efficiency should be benchmarked from other well performing hospitals.

