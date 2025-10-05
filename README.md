# Coupon Acceptance Analysis

UC Berkeley Professional Certificate in ML & AI - Assignment 5.1

## Overview

This project analyzes mobile coupon acceptance behavior using survey data from Amazon Mechanical Turk. The analysis explores what factors influence whether drivers accept coupons delivered to their phones in various driving scenarios.

## Dataset

- **Source:** UCI Machine Learning Repository
- **Size:** 12,684 observations (after cleaning)
- **Coupon Types:** Restaurant (<$20), Coffee House, Carry Out, Bar, Restaurant ($20-50)
- **Features:** Demographics, driving context (time, weather, passenger, destination), visit frequency

## Key Findings

### Overall Acceptance
- **57%** of drivers accept coupons
- Acceptance varies significantly by coupon type and context

### Bar Coupons
- **Visit frequency dominates:** 76% acceptance for frequent bar-goers (>3/month) vs 37% for infrequent visitors
- Age matters when combined with frequency: 55% acceptance for age 25+ with regular visits
- **Key insight:** Coupons reinforce existing habits rather than create new behavior

### Coffee House Coupons  
- **Time-sensitive:** 63% acceptance at 10AM (peak) vs 41% at 6PM
- **Social context matters:** 60% with friends vs 43% alone
- Weaker frequency effect than bars (+23pp vs bars' +39pp)
- **Key insight:** Convenience and social experience drive acceptance

## Methodology

1. **Data Cleaning:** Removed duplicates, dropped 99% missing 'car' column, handled missing frequency data
2. **Exploratory Analysis:** Distribution analysis, acceptance rates by feature
3. **Comparative Analysis:** Group comparisons using statistical summaries and visualizations
4. **Visualization:** Bar charts, histograms, multi-panel comparisons

## Technologies

- Python 3.11
- pandas, numpy - data manipulation
- matplotlib, seaborn - visualization
- Jupyter Notebook - analysis environment
