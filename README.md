# MediTrack-Hospital-Operations-Analysis
A Power BI healthcare analytics project transforming a flat-file dataset into a scalable star-schema data model to track hospital KPIs and patient outcomes
# Project Overview

MediTrack Global Health is an international healthcare organization modeled after the UK's National Health Service (NHS). It operates hospitals and medical centers across ten countries, providing a wide range of services including patient care, consultations, diagnostics, and treatments.
Problem Statement
Previously, MediTrack’s operational data was stored in a single flat file that combined patient details, doctor information, hospital data, and financial records. As the organization grew across 10 countries, this flat file became inefficient, leading to:  

 Potential data duplication.  

 Poor performance in Excel.  

Difficulty in monitoring patient outcomes and comparing efficiency across different hospitals.

# Aim of the Project
The primary goals of this project are:Data Transformation: Convert raw operational data into a structured and normalized data model.  Scalability: Create a scalable model that facilitates easy tracking of Key Performance Indicators (KPIs).  Strategic Insights: Provide management with actionable insights to improve hospital performance and financial outcomes.

# Tools and Technology
Power BI: Used for data modeling, DAX calculations, and visualization.  Power Query: Used for data cleaning and transformation.  DAX (Data Analysis Expressions): Used to create complex measures and KPIs.  Excel: Source of the initial raw operational data.

# Data Model Architecture
The project involved normalizing the flat file into a Star Schema to optimize performance. The model consists of:  Fact Table: Contains transactional data such as Admission Dates, Costs (Treatment, Medication, Diagnostic), Revenue Billed, and Length of Stay.  Dimension Tables: * PatientDim: Patient details (Name, Gender, Age).  DoctorDim: Staff information and specialties.  HospitalDim: Hospital locations and country data.  DepartmentDim: Department names and IDs.  CalendarDim: For time-series analysis. 

# Key Measures & KPIs (DAX)
To support business decisions, several DAX measures were developed:  

Total Admissions: Volume of patients handled.

Average Length of Stay: Efficiency of patient discharge.

Total Revenue & Net Income: Financial health analysis.

Recovery Rate: Quality of care and patient outcomes.

# Project Workflow

Data Acquisition: Downloaded and inspected the Excel healthcare dataset.  


Data Modeling: Imported the file into Power BI and established relationships between fact and dimension tables.  


DAX Calculations: Created custom measures to track operational and financial performance.  


Reporting: Developed an interactive dashboard to extract actionable insights for hospital management.
