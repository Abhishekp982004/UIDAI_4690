# UIDAI Biometric Update Analysis – Data Hackathon 2026

## Overview

This repository contains the analytical work developed for the **UIDAI Data Hackathon 2026**, focusing on understanding biometric update behaviour across temporal, age-wise, and regional dimensions.

The objective of this project is to identify operational patterns, anomalies, and regional disparities in Aadhaar biometric update activity and propose data-driven interventions to support efficient and citizen-centric biometric revalidation.

---

## Problem Statement

Analyzing temporal, age-wise, and regional patterns in Aadhaar biometric update activity to identify anomalies, operational inefficiencies, and age-transition bottlenecks, and proposing data-driven interventions to support timely, efficient, and citizen-centric biometric revalidation.

---

## Dataset Used

- **Dataset Name:** Aadhaar Biometric Update Dataset  
- **Publisher:** Unique Identification Authority of India (UIDAI)  
- **Source Platform:** Open Government Data Platform (data.gov.in)  
- **Data Type:** Aggregated and anonymized public data  
- **Coverage:** Up to 31 December 2025  

### Key Attributes
- Date of biometric update  
- State, District, and PIN Code  
- Biometric updates for age group 5–17  
- Biometric updates for age group 18+  

No personally identifiable information is included in the dataset.

---

## Methodology

The analytical pipeline consists of the following stages:

1. **Data Ingestion and Consolidation**
   - Multiple CSV files merged into a unified dataset

2. **Data Cleaning and Preprocessing**
   - Date standardization using Indian day-first format
   - Removal of invalid or incomplete records
   - Geographic name normalization

3. **Feature Engineering**
   - Month and year extraction
   - Total biometric update computation
   - Age-group-wise aggregations

4. **Temporal Analysis**
   - Monthly trend analysis
   - Identification of peak and low-demand periods

5. **Age-wise Analysis**
   - Participation comparison between age groups
   - Stability assessment across months

6. **Anomaly Detection**
   - Rolling Z-score–based detection
   - Interquartile Range (IQR) validation
   - Median Absolute Deviation (MAD) for regional robustness

7. **Regional Analysis**
   - State-level aggregation
   - Identification of inter-state variability and anomalies

---

## Key Analyses Performed

- Month-wise biometric update trend analysis  
- Age-group participation distribution analysis  
- Temporal anomaly detection on daily update volumes  
- Regional outlier detection across states  
- Comparative assessment of age-wise participation patterns  

---

## Outputs Generated

- `M3_temporal_outliers.csv`  
  - Contains dates flagged as anomalous along with deviation indicators

- `M3_regional_outliers_FINAL.csv`  
  - Contains states identified as regional outliers with supporting metrics

---

## Key Findings

- Biometric update demand exhibits strong seasonal variation
- Age-wise participation remains stable across months
- Significant inter-state heterogeneity exists in update volumes
- Uniform national operational strategies may be suboptimal
- Temporal anomalies indicate short-term operational stress periods

---

## Proposed Solutions

- Time-specific resource deployment during peak-demand periods
- State-specific operational planning based on update intensity
- Targeted awareness programs for age-transition biometric revalidation
- Continuous monitoring using anomaly detection frameworks

---

## Team

**Team ID:** UIDAI_4690  

- Bhuvi Prashanth   
- Abhishek P  
- Abhranshu Sarkar  
- Adarsh V  
- Aditya D Rao  

---

## Notes

- This repository is provided for reference and reproducibility.
- The complete project report was submitted as a consolidated PDF as part of the hackathon requirements.
- The dataset used is publicly available on the UIDAI Open Government Data Platform.

---

## License

This project is developed for academic and research purposes as part of the UIDAI Data Hackathon 2026 using publicly available government data.
