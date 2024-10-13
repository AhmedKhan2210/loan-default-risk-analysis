# Loan Default Risk Analysis

## Project Overview
This project focuses on evaluating credit risk in lending by analyzing past loan data to better understand factors that lead to loan defaults. 
By carefully examining variables such as loan amount, loan type, interest rates, and borrower characteristics (e.g., age, credit score, region), 
the project categorizes loans into different risk levels. Feature engineering, such as the introduction of a “Risk Category,” provides a deeper insight into loan default trends, 
supporting more informed lending decisions without using machine learning models.

## About Data

'ID','Year' ,'Gender'-: Represents ID of customer (148670 unique IDs), gender we have Male,Female, joint,& gender missing.
‘'Loan_limit': We have two type Fixed/Confirmed and Not Fixed/Not Confirmed
'loan_type', 'loan_purpose',: 3 type of loan and 4 type of loan purpose
'business_or_commercial', 'loan_amount', 'rate_of_interest','property_value','income', 'Credit_Score', 'age','Region'
'Upfront_charges': Down payments done by applicant
'Credit_type', Co-applicant_credit_type': 4 type ( 'EXP' 'EQUI' 'CRIF' 'CIB')
'LTV', 'Status': 0 Represents Non-Default loans and 1 Represents Defaulted loans


## Key Features

#Comprehensive Data Analysis:

Analyzes 150,000 loan records with 20 fields, focusing on factors like loan amount, interest rates, credit scores, and LTV ratios.
Data Preparation Techniques:

Addresses missing values and outliers to ensure data integrity for accurate analysis.

Feature Engineering:

Introduces the "Risk Category" variable to classify loans into risk levels based on LTV, credit score, and income.
Exploratory Data Analysis (EDA):

Reveals key patterns in borrower demographics and loan preferences, highlighting relationships between loan characteristics and default rates.

Visualizations:

Uses heatmaps, scatter plots, and bar graphs to effectively communicate insights from the analysis.

Statistical Analysis:

Calculates effect sizes and conducts statistical tests to evaluate factors influencing default rates.

Actionable Recommendations:

Provides strategies for improved risk assessment, such as focusing on LTV ratios and implementing stricter credit assessments.

## Conclusion
Most of the borrowers belong to the lower to middle-income class and are primarily from the North and South regions. Their first preference for loans is Type 1, and the preferred occupancy type is PR. The majority of the loans are for small amounts, with the purpose being P3. The property values typically range between $200,000 to $400,000, with the standard category being the most preferred
Equi credit type has almost 100% default rate, and among all credit type sub_cat occupancy type IR on top  and SR has 2nd most defaulted loan, while checking co applicant credit type CIB is good, EXP has high default rate
As the Age increases default rate increases, In gender where the gender is missing has high default rate, Business loans are more likely to default
High and very high LTV 78 to 84% chances to default, purpose p1 has 31% default rate where as property category standard and economy more likely to default.
Surprisingly credit score has no impact on default rate

## Recommendations

Focus on LTV Ratio: Lenders should prioritize evaluating loan applications based on the LTV ratio, as it has a significant impact on loan defaults. Should increase downpayment and introduce insurance to such loans

Stricter Credit Assessments for Certain Credit Types: Implement stricter lending policies for loans using EQUI and EXP credit types, it is better to discontinue EQUI. Encourage the use of CIB credit type for co-applicants.

Reevaluate Loan Policies for Older Borrowers: Since older borrowers tend to default more, consider adding age-based risk adjustment factors to the loan approval process.Ensure that gender data is collected accurately,because where gender missing those loans are likely to default.

Improve Risk Categorization: Use the derived risk categories (Very Low Risk to Extremely High Risk) to tailor loan offerings and risk mitigation strategies for high-risk borrowers.Introduce more stringent evaluation criteria for business loans

Implement stricter credit assessments for Loan Type 1 applicants, especially for small loans. For Occupancy Type IR, apply stricter approval criteria, such as higher income requirements or larger down payments. This should be coupled with continuous monitoring to mitigate risk.

Introduce specialized products for Purpose P1 loans with stricter approval processes, perhaps offering lower loan limits or shorter repayment terms to minimize risk.Assess the property value and adjust the lending terms accordingly for these categories, perhaps requiring lower LTV ratios, better credit scores, or additional collateral.

