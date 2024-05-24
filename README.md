# GEOG5990M_Project
Employs Python to examine spatial patterns and relationships between health characteristics, substance abuse, and healthcare access in Stockport, UK


**The GitHub Repository contains:**

**The .pynb project file. (main)**

3 CSV files containing information on Stockport Hospital Attendances and Admissions, Stockport Smoking and Asthma Prevalence, and Stockport Local Health Characteristics.


1 html (pynb to HTML) file for easier accessibility

1 Stockport shapefile (with supported files). The original shapefile was of all of the UK which was >600 mb. Due to data constraints as both GitHub as well as Minerva (official submission portal) allows file size upto 100 mb, Stockport boundaries were extracted with the help of a GIS software.

Link for the original UK Shapefile: https://statistics.ukdataservice.ac.uk/dataset/2011-census-geography-boundaries-lower-layer-super-output-areas-and-data-zones

Stockport Hospital Attendances and Admissions https://datamillnorth.org/dataset/ep6pr/stockport-hospital-attendances-and-admissions

Stockport Smoking and Asthma Prevalence https://datamillnorth.org/dataset/2jq60/stockport-smoking-and-asthma-prevalence

Stockport Local Health Characteristics https://datamillnorth.org/dataset/20j06/stockport-local-health-characteristics





**The README file contains**:
1. What the Code Aims to Do
2. Project Decisions
3. Intended Audience
4. Abstract, Discussion and Conclusion for the Project


**1. What the Code Aims to Do**
Add, summarize, and preprocess three datasets.
Conduct an extensive spatial analysis.




**2. Project Decisions**
The project adopts a report-style format for presenting the Python-based spatial analysis work. The visual data processing approach involves loading the Stockport shapefile, joining it with a CSV dataset, and then extracting specific LSOAs which aligns with standard GIS (Geographic Information Systems) workflows.



The project is divided into five parts:
•	Section 1-3: Adding, summarizing, and preprocessing the three CSV datasets
•	Section 4-5: Main analysis



An html file has been included in the repository for easy of accessibility for early users, or easy computational requirements.




**Important Note**:
The shapefile for the whole of the UK is large and will need some time to load, so hold tight and get a coffee in the meanwhile. It could have been filtered out first using a GIS software but using the jupiter notebook was decided to keep it a little challenging.




**3. Intended Audience**
The intended audience for this project includes:
•	Public health officials and policymakers focused on improving population health outcomes and reducing health disparities
•	Healthcare providers and administrators interested in understanding the spatial distribution of health issues and healthcare access in their service areas
•	Researchers in the fields of public health, epidemiology, health geography, and social determinants of health
•	Community organizations and advocates working to address health inequities and promote health and well-being in their local areas
•	Data scientists and spatial analysts interested in applying Python for health-related spatial analysis




**4. Abstract**
This data science project employs Python to examine the spatial patterns and relationships between various health characteristics, substance abuse (alcohol and smoking), and healthcare access in Stockport, UK at the Lower Layer Super Output Area (LSOA) level. The analysis combines multiple datasets on hospital admissions, smoking and asthma prevalence, chronic health conditions, and GP registration. Exploratory data analysis reveals correlations between smoking prevalence, asthma cases, and alcohol-related hospital admissions. Higher GP registration rates are associated with lower rates of most chronic health conditions and substance abuse. Spatial mapping using the Getis-Ord Gi* statistic identifies clusters of LSOAs with high and low GP registration rates. The findings suggest that improved access to primary care through GP registration may help prevent and manage chronic health issues and substance abuse in the population. This study provides valuable insights for public health officials and policymakers to target interventions in areas with poorer health outcomes and limited healthcare access.
The analysis assumes a basic understanding of statistical concepts, spatial analysis techniques, and interpreting data visualizations. Some familiarity with the UK census geography and administrative boundaries would also be beneficial for contextualizing the findings.




**Discussion and Conclusion**
From the Getis-Ord Gi* map(	Section 5.2), it can be seen that GP registration rates form distinct geographic clusters. There are pockets of low GP registration (blue/purple areas) in central and northern regions, while southern areas generally have medium to high registration rates (yellow/orange/red). This suggests spatial disparities in access to primary care.
Looking at the heat map correlation(in Section 4.2), most health conditions appear to have an inverse relationship with GP registration rates. As GP registration increases (moving right on the x-axis), the prevalence of conditions like COPD, CHD, hypertension, anxiety, depression, asthma, diabetes, cancer, stroke, and smoking tends to decrease (moving down on the y-axis). The trend lines have a negative slope, confirming this inverse relationship.
However, atrial fibrillation, chronic kidney disease, and dementia seem to slightly increase with higher GP registration, possibly due to these conditions being more common in older populations who may be more likely to be registered.
In conclusion, the geographic analysis reveals clusters of low GP registration that may indicate barriers to primary care access in certain areas. The scatterplots demonstrate that, for most chronic conditions analysed, prevalence appears to be inversely related to GP registration rates. This suggests that populations with lower rates of registration with a GP generally experience higher rates of several chronic health issues. Improving primary care registration and access could potentially help in preventing and managing these conditions better. However, the positive association seen with a few conditions underscores the complexity of these relationships and the need for further research to understand the nuances and develop targeted interventions.
