# Healthcare-Analytics
https://github.com/user-attachments/assets/469b73d5-2a32-4542-83c1-94d3e044471d

# Project Overview
In pursuit of excellence in patient care and operational performance, NovaCare Hospitals aims to enhance operational efficiency by analyzing key processes across admissions, billing, and follow-up workflows. This project consolidates data from various departments, including admissions, billing, and follow-up services, to provide a holistic view of hospital operations. 

#Data Description
The NovaCare Hospitals dataset is structured to represent core hospital operations and clinical workflows. It includes patient visits, diagnoses, procedures, billing, and provider details, enabling deep analytical insights through Power BI.

![Healthcare-Analytics](Images/datamodel.jpg)
### patients
Contains demographic data of patients.
- `Patient ID`, `Patient Name`, `Age`, `Gender`, `City ID`

### date
Calendar table for time intelligence in reporting.
- `Date`, `Day_Num`, `Day_Type`, `Month`, `Month_Num`

### visits
Central fact table capturing hospital visit data.
- `Admitted Date`, `Discharge Date`, `Diagnosis ID`, `Procedure ID`, `Department ID`, `Insurance ID`
- `Length of Stay`, `Treatment Cost`, `Medication Cost`, `Room Charges`
- `Insurance Coverage`, `Referral Source`, `Service Type`, `Payment Status`
- `Patient Satisfaction Score`

### Insurance
Provides insurance-related metadata.
- `Insurance ID`, `Insurance Provider`

### Departments
Describes hospital departments.
- `Department ID`, `Department`

### Procedures
Defines procedures performed during patient visits.
- `Procedure ID`, `Procedure`

### Diagnoses
Stores diagnosis information.
- `Diagnosis ID`, `Diagnosis`

### Providers
Captures details about healthcare providers.
- `Provider ID`, `Provider Name`, `Age`, `Gender`, `Nationality`

### Cities
Geographic dimension for mapping patients.
- `City ID`, `City`, `State`

### _calculations
This table contains all custom **DAX measures** used in analysis.
- `Total Treatment Cost`, `Total Medication Cost`, `Total Insurance Coverage`, `Total Room Charges`, etc.

#
