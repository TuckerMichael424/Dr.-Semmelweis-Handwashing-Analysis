# Dr.-Semmelweis and the Impact of Handwashing - A Data Analysis Project in R
An analysis of Dr. Semmelweis's discovery and implementation of handwashing and how drastically it affected the mortality rate in the medical industry. 

## Overview
This project analyzes the impact of Dr. Ignaz Semmelweis's handwashing discovery on maternal mortality rates in 19th-century Vienna General Hospital. The analysis demonstrates how a simple hygiene intervention revolutionized medical practices and saved hundreds of lives.

## Business Context
This analysis was conducted to support Modern Health Medical Center's annual Hand Hygiene Awareness Week. The goal is to use historical data to demonstrate the critical importance of handwashing in preventing infections and improving patient safety, providing evidence-based support for training programs and awareness campaigns.

## Dataset
The data comes from DataCamp's Dr. Semmelweis Handwashing Analysis project and includes two main dataframes:
- **yearly_deaths_by_clinic.csv**: Annual birth and death records for Clinic 1 and Clinic 2 (1841-1846)
- **monthly_deaths.csv**: Monthly birth and death records (1841-1849)

## Methodology

### Data Processing
- Created a `proportion_deaths` field calculating death-to-birth ratios
- Added a boolean `handwashing_started` field (threshold: June 1, 1847)
- Parsed date fields to extract month and year for granular analysis
- Created a `season` field to analyze seasonal patterns (Winter, Spring, Summer, Fall)

### Analysis
- Statistical analysis including mean, median, range, and standard deviation of death proportions
- Comparative analysis before and after handwashing implementation
- Seasonal pattern analysis to understand mortality fluctuations
- Visual representations using ggplot2

## Key Findings

### Handwashing Impact
The implementation of handwashing resulted in an **89% reduction** in the proportion of deaths:
- Before handwashing: Average death rate of 10.5%
- After handwashing: Average death rate of 2.1%

### Seasonal Patterns
Despite the dramatic improvement from handwashing, seasonal analysis revealed notable mortality spikes between September and March. Several factors may have contributed to these patterns:
- Inadequate sanitary infrastructure in 19th-century hospitals
- Cultural beliefs and norms surrounding medical practices
- Limited medical knowledge of germ theory
- The lingering effects of the [Little Ice Age](https://en.wikipedia.org/wiki/Little_Ice_Age), with colder temperatures potentially exacerbating health conditions

## Visualizations
The analysis includes:
1. Yearly death proportions by clinic (stacked area chart)
2. Monthly death proportions with handwashing threshold (line chart with ribbon)
3. Seasonal breakdown of death proportions before/after handwashing (faceted bar chart)

## Conclusion
Dr. Semmelweis's discovery of handwashing revolutionized medical practice and dramatically improved patient outcomes. While seasonal factors continued to influence mortality rates, the data clearly demonstrates that this simple intervention laid the groundwork for modern infection control practices. This historical evidence reinforces the critical importance of hand hygiene in healthcare settings today.

## Technologies Used
- R Programming Language
- Tidyverse (dplyr, ggplot2, lubridate)
- Scales package for percentage formatting
- Jupyter Notebook via Kaggle

## Future Research Directions
- Investigate correlation between temperature data and mortality spikes
- Compare mortality patterns across different European clinics
- Analyze the role of hospital infrastructure in patient outcomes

## Acknowledgments
- DataCamp for the original project framework
- Kaggle for the notebook environment
- Dr. Ignaz Semmelweis, whose pioneering work continues to save lives

---

*"The truth will set you free, but first it will make you miserable." - Dr. Ignaz Semmelweis*
