# Financial Risk Analysis and Business Recommendations

This repository provides an in-depth analysis of financial risk factors across various demographic groups based on attributes like income, marital status, house and car ownership, and profession. The goal is to derive actionable insights and business recommendations to help financial institutions tailor their products and services effectively.

## 📊 Project Overview

The project employs descriptive statistics, univariate and multivariate analysis, outlier detection, and correlation analysis to understand the distribution of financial risk among individuals. We have also developed targeted business recommendations for different age groups, professions, income levels, and other demographic factors based on the insights derived.

## 📂 Table of Contents
- [Data Summary](#data-summary)
- [EDA](#EDA)
  - [Descriptive Statistics](#descriptive-statistics)
  - [Univariate Analysis](#univariate-analysis)
  - [Outlier Detection](#outlier-detection)
  - [Multivariate Analysis](#multivariate-analysis)
- [Business Recommendations](#business-recommendations)


## 📄 Data Summary


## 🔍 EDA

### Descriptive Statistics
1. **Income and Experience**: Large ranges suggest potential outliers.
2. **CURRENT_HOUSE_YRS**: Narrow range, possibly indicating data bias.
3. **Risk_Flag Distribution**: Strong imbalance, with a majority in the low-risk category.

### Univariate Analysis
- **Income**: Nearly uniform distribution with minor fluctuations; wide range indicates potential outliers.
- **Age**: Even distribution from ages 21 to 79, with no age group dominating.
- **Experience**: Diverse levels of experience with a wide variation in career lengths.
- **CURRENT_JOB_YRS**: Right-skewed, with most individuals in shorter job tenures.
- **CURRENT_HOUSE_YRS**: Highly concentrated between 10-14 years, raising questions about data relevance.
- **Risk_Flag**: Highly imbalanced, dominated by 0 (low-risk), which will need handling during pre-processing.

### Outlier Detection
- **Income**: Identified as a feature with potential outliers.
- **Action**: Perform outlier detection and handling to manage extreme values effectively.

### Multivariate Analysis

#### Correlation with Risk_Flag
- **Low Correlation**: No strong correlations between individual numerical features and `Risk_Flag`.
- **Features like Experience, Age, and CURRENT_JOB_YRS**: Although they have low correlation, they might contribute useful information in a predictive model.

#### Feature Correlations
- **Experience, Age, CURRENT_JOB_YRS**: Retained for potential minor contributions in machine learning models.
- **Redundancy Handling**: Additional feature importance testing to eliminate redundancy without losing accuracy.

#### Categorical Feature Correlations with Risk_Flag
- **Marital Status**: Single individuals tend to have a higher risk than married ones.
- **House Ownership**: Higher risk for renters compared to owners.
- **Car Ownership**: Moderate relevance, with balanced risk distribution.
- **Profession**: Varying levels of risk across professions, indicating high relevance.

## 💼 Business Recommendations

Based on the above insights, here are targeted business recommendations for different demographic segments:

### Age Group-Based Recommendations

- **Ages 0-25**:
  - **Savings and Starter Investment Products**: Offer long-term savings and small-scale investments to encourage financial habits.
  - **Financial Education Programs**: Educate on basic financial management to build positive habits early.

- **Ages 26-35**:
  - **Consumer Loans**: Provide flexible loans for vehicles or home renovations to support lifestyle needs.
  - **Basic Insurance**: Health or accident insurance for initial protection.

- **Ages 36-50**:
  - **Financial Consulting**: Offer services to manage assets and plan for future financial stability.
  - **Comprehensive Insurance**: Provide health, life, and property insurance options tailored to this age group’s complex needs.

- **Ages 51-65 and 66+**:
  - **Retirement Planning**: Introduce low-risk savings or retirement plans.
  - **Long-term Health Insurance**: Offer products focused on health and long-term care needs.

### Profession-Based Recommendations

- **High-Risk Professions** (e.g., Police Officer, Chartered Accountant, Army Officer, Scientist, Civil Engineer):
  - **Comprehensive Insurance**: Provide life and accident insurance to manage high occupational risks.
  - **Stricter Loan Requirements**: Implement secure credit terms or collateral-based loans.

- **Low-Risk Professions** (e.g., Librarian, Politician, Economist, Petroleum Engineer, Technology Specialist):
  - **Premium Investment Products**: Offer high-yield investment options.
  - **Low-Interest Loans**: Provide lower interest rates on loans as a reward for stable risk profiles.

### Income Level-Based Recommendations

- **Low Income**: Focus on financial literacy and provide access to basic financial services.
- **Middle Income**: Offer moderate-risk management products like insurance and investment.
- **High Income**: Promote wealth management and premium services.

### Marital Status and House Ownership-Based Recommendations

- **Single Renters**: Encourage transitioning to homeownership with supportive financing programs.
- **Married Couples**: Target with family insurance and joint financial planning products.

### Ownership-Based Recommendations

- **Renters without Cars**: Target with homeownership transition programs and renter insurance.
- **Renters with Cars**: Offer car insurance and homeownership programs.

## 🚀 Next Steps

1. **Outlier Detection**: Use robust methods to handle outliers in Income and Experience.
2. **Class Balancing**: Address `Risk_Flag` imbalance using methods like SMOTE.
3. **Feature Engineering**: Apply transformations for features with skewed distributions.
4. **Predictive Modeling**: Use the insights for model training to predict financial risk and recommend suitable products.

