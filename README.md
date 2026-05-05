# MediTrack-Hospital-Operations-Analysis
A healthcare analytics project built in Power BI that transforms raw operational data into a scalable star-schema model, enabling KPI tracking across hospitals and improving visibility into patient outcomes, efficiency, and financial performance.

# Project Overview
MediTrack Global Health is an international healthcare provider operating across 10 countries, delivering services such as patient care, diagnostics, and treatment.

As the organization expanded, its data remained in a single flat file combining patient, hospital, doctor, and financial information. This created major limitations:

1. Data duplication and inconsistency

2. Poor performance in Excel

3. Limited ability to track KPIs and compare hospital performance

# Objectives
1. Transform raw healthcare data into a normalized, scalable model

2. Enable efficient tracking of operational and financial KPIs

3. Provide actionable insights to improve hospital performance and patient outcomes

# Tools & Technologies
1. Power BI (data modeling and visualization)

2. Power Query (data cleaning and transformation)

3. DAX (calculated measures and KPIs)

# Excel (data source)

Data Model (Star Schema)
The flat dataset was restructured into a star schema to improve performance and scalability.

Fact Table: Admissions, costs (treatment, medication, diagnostics), revenue, length of stay

Dimension Tables:

PatientDim (demographics)

DoctorDim (staff and specialties)

HospitalDim (locations and countries)

DepartmentDim (clinical units)

CalendarDim (time intelligence)

# Key Measures (DAX)
	Total Admissions
"Total Admissions"=COUNT(FactAdmissions[PatientID])

	Average Length of Stay
"Avg LOS"=AVERAGE(FactAdmissions[LengthOfStayDays])

	Total Revenue
"Total Revenue"=SUM(FactAdmissions[RevenueBilled])

	Net Income
"Net Income"=SUM(FactAdmissions[RevenueBilled])-SUM(FactAdmissions[TotalExpenses])

	Recovery Rate
"Recovery Rate"=DIVIDE([RecoveredPatients],[TotalAdmissions])


# Dashboard Features
Global view of hospital performance across 10 countries

1. Drill-down by hospital, department, and specialty

2. Time-series analysis of admissions and occupancy trends

3. Cost and revenue breakdown by category

4. Patient outcome tracking (Recovered, Referred, Ongoing, Deceased)

# Key Insights & Business Impact
1. Identified high patient volumes in key regions (UK, US, India), supporting targeted staffing and resource allocation

2. Detected bottlenecks in Emergency and Cardiology departments, enabling data-driven workforce redistribution
3. ![Dashboard](images/screenshot 2026-05-05 145951.png)

4. Highlighted high bed occupancy in Oncology and Neurology, informing infrastructure expansion decisions

5. Revealed major cost drivers (medication vs diagnostics), supporting supplier negotiation strategies

6. Tracked readmission patterns to identify ineffective treatments, improving clinical protocols

7. Analyzed revenue vs cost gaps to identify the most financially sustainable specialties


