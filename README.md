# Lending Club Case Study
### The objective of this case study is to identify the driving factors behind loan defaults. By understanding these factors, the company can:
- Reduce the number of risky loans issued
- Minimize financial losses due to defaults
- Implement strategic actions for high-risk applicants such as 
    - Denying loans
    - Adjusting loan amounts
    - Modifying interest rates

## Table of Contents
* [General Information](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
1. [Business Overview](https://github.com/vikrant19y/LendingClubCaseStudy/blob/main/Lending_Club_CaseStudy.ipynb)
    1. Business Understanding: A consumer finance company that specializes in providing various types of loans to urban customers. The company needs to make informed decisions regarding loan approvals based on the applicant's profile. The primary risks involved in this decision-making process are:
        - Loss of Business Opportunity: If a loan is denied to an applicant who would have repaid it.
        - Financial Loss: If a loan is approved for an applicant who ends up defaulting.

    2. Business Objective: A dataset is provided that contains historical information about past loan applicants, including whether they defaulted. The aim is to identify patterns and attributes that indicate a higher likelihood of default. This understanding will help the company take preemptive actions.
  
2. [Data Acquisition](https://github.com/vikrant19y/LendingClubCaseStudy/blob/main/Lending_Club_CaseStudy.ipynb)
    1. Data is provided for 5 years from 2007 to 2011 in CSV format.
  
3. [Data Preparation](https://github.com/vikrant19y/LendingClubCaseStudy/blob/main/Lending_Club_CaseStudy.ipynb)
    1. Data Cleaning
        - Dropping rows/columns that are completely null
        - Dropping irrelevent columns. The columns that do not contribute to the analysis
        - Missing values treatment
        - Handling outliers
        - Filtering data
    2. Data Transformation
        - Standardize numbers
        - Derive new columns

4. [Exploratory Data Analysis(EDA)](https://github.com/vikrant19y/LendingClubCaseStudy/blob/main/Lending_Club_CaseStudy.ipynb)
    1. Univariate Analysis
        - Categoriacal
        - Numerical
    2. Segmented Univariate Analysis
    3. Bivariate Analysis
    4. Multivariate Analysis
    5. Statistical Analysis


## Analysis

## Summary
1. Overall 14.5% loans were charged-off in the given dataset.
2. There is an exponential increase in number of loans offered from year 2007 to 2011
3. **TODO Add summary of credit loss and profit %**

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
***Note: Conclusions are ordered based on their weightage and how strognly they contributed to the analysis.***
1. **Purpose:** The purpose of loans taken for _small_business_ and _renewable_energy_ are more risky. Default rates are **28%** and **20%** respectively. While the other purposes are relatively less risky, we observed more credit loss for _debt_consolidation_ purpose which is ~ $14M because volume is high in this purpose.
2. **Revolving Utilization:** Higher utilization rates correlate with higher default rates. The highest charged-off rate in this segment is **20%** for the customers who utilize their available credit 80%-100%. Credit loses are also proportional to the utilization rates.
3. **DTI (Debt-to-Income):** Higher DTI ratios lead to higher default rates. Charged-off rate increases starting from 13% to 17%. Higher DTI ratios lead to higher charged-off rates and increased credit losses.
4. **Annual Income:** Higher income correlates with lower default rates. Charge-off rate decreases from 18% (1k-30k) to 11% (90k-150k). Credit loss is highest for income range 30k-60k ~ $11M.
5. **Loan Amount:** Larger loan amounts correlate with higher default rates. Charge-off rates rising from 13% for loan amount between 0-10k to 28% for loan amount between 30k-40k.
6. **Home Ownership:** Category OTHER has higher default rate 19%.
7. **Employment Length:** Default rate almost same across all levels approximately ~15%. Out of all 10+ years people are defaulting slightly more than others with 16%. But, there is huge credit loss in this category though the difference is just 1% because of volume.
8. **Verification Status** Even verified customers are more likely to default at the rate of 17% and credit loss is ~ $12.5M.
9. **Term:** 60 months loan term has more default rate compared to 36 months. Charged-off percentage is 26% for 60 months and 11% for 36 months.
10. **Grade:** Lower loan **grade**s have higher default rate. The risk level increases from grade A(6%) to grade G(35%).
11. **Installment:** Higher monthly installments correlate with higher default rates. Charged-off rate increases from 14% (0-300) to 21% (900-1300).
12. **Funded Amount:** Larger funded amounts correspond to higher default rates. The charged-off rate increases from 13% (for amounts between 0-10k) to 28% (for amounts between 30k-40k).
13. **Interest Rate:** Interest rate is positively correlated with default rate. Charged-off rate is 7% for 5-10% and 39% for 20-25%.
14. **Total Accounts:** Total accounts show stable default rates with slight variations. Charge-off rate is relatively stable around 14-15% across most ranges.
15. **Public Records:** People with derogatory/bankruptcy history are more likely to default. But, loans offered to such customers is also very less.



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.12
- Pandas 2.2.2
- NumPy 1.26.4
- MatplotLib 3.8.4
- Seaborn 0.13.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project was inspired by live session of IITB on EDA
- UpGrad tutorials on Exploratory Data Analysis (EDA) on the learning platform


## Authors 
- [Chandra Sekhar Kommuri](@chandrakommuri)
- [Vikrant Yadav](@vikrant19y)


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
