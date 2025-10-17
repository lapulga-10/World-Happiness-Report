# Aspirin, the Miracle Drug? 💊

This project investigates the effectiveness of regular aspirin intake in preventing heart attacks. Using data from a large-scale experimental study, this analysis employs contingency tables, measures of association, and the chi-squared test to determine if there is a statistically significant relationship between taking aspirin and the incidence of heart attacks.

## About The Project
Aspirin is widely used for pain relief and anti-inflammatory purposes, and is also commonly prescribed to prevent heart attacks and strokes. This project analyzes data to answer the key question:

**Does aspirin significantly reduce the risk of a heart attack?**

The analysis explores:  
- Distribution of heart attacks among different groups (aspirin vs. placebo, smokers vs. non-smokers, and different age groups).  
- Strength of association between aspirin intake and heart attack events using Risk Ratio (RR) and Odds Ratio (OR).  
- Statistical significance of the association using a chi-squared ($\chi^2$) test of independence.

## Dataset
The analysis is based on the `Aspirin.csv` dataset, compiled from an unpublished experimental study conducted in 1993.  

**Study Design:**  
- Double-blind experiment where male participants were randomly assigned either an aspirin or placebo tablet every two days for five years.  
- **Size:** 20,021 observations, no missing values.  
- **Variables:**  
  - `Group`: Tablet type ("Aspirin" or "Placebo")  
  - `HeartAttack`: Whether the participant had a heart attack ("Yes" or "No")  
  - `Smoking`: Smoking status ("Smoker" or "Non-Smoker")  
  - `Age`: Participant age, categorized from "61" to "65"  

## Statistical Methods
- **Two-Way Contingency Tables:** Summarizes joint frequency distributions of two categorical variables (e.g., Group vs HeartAttack).  
- **Measures of Association:**  
  - Risk Ratio (RR): Risk of heart attack in aspirin group relative to placebo.  
  - Odds Ratio (OR): Odds of heart attack in aspirin group relative to placebo.  
- **Chi-Squared ($\chi^2$) Test:** Tests for significant association between two categorical variables. Null hypothesis: variables are independent.

## Key Findings 📈
- **Aspirin’s Protective Effect:**  
  - Heart attack rate: 2.32% in aspirin group vs 5.57% in placebo.  
  - Risk Ratio (RR) = 0.417 (~58% reduction in risk).  
  - Odds Ratio (OR) = 0.403 (~60% reduction in odds).  
- **Statistical Significance:**  
  - Chi-squared test p-value < 2.2e-16 → strong evidence of association between aspirin and reduced heart attacks.  
- **Other Factors:**  
  - Smokers had nearly double the heart attack rate compared to non-smokers.  
  - Heart attack rates were consistent across ages 61–65.  

## Technologies Used
- **Language:** R  
- **Packages:**  
  - `epitools` for epidemiological calculations and contingency tables  
  - `dplyr` for data manipulation  
  - `ggplot2` for data visualization  

## How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/aspirin-heart-attack-study.git


2. Open the project in RStudio.

Install required packages:

install.packages(c("epitools", "dplyr", "ggplot2"))


3. Run the analysis script to generate results and visualizations. Ensure Aspirin.csv is in your working directory.

Author

Rahul Ramesh Vishwakarma
