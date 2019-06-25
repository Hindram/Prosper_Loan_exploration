# Prosper Loan Data Exploration
## by Hind Al Ramah


## Dataset

This data set contains 113,937 records of loans along with 81 variables on each loan, such as loan amount, interest rate, borrower income, and many others. Our exploration will foucs on only 10 to 13 variables. After dropping some irrelevant features of our investigation, we have only 46 variables. The data set includes 31 float, 4 int, and 11 object variables.

### Main features:
##### 'CreditGrade', 'Term','BorrowerAPR', 'InterestRate', 'ProsperRatingAlpha', 'LoanStatus' and 'LoanOriginalAmount'.

### Support features:
##### 'MonthlyLoanPayment', 'IncomeRange', 'BorrowerState', 'ProsperRatingNumeric' and more.
 
## Summary of Findings

### Univariate Exploration
- Loan Status: most loans were current and least were past due.

- ProsperRatingAlpha: the most risk scale fills under C, B, and A respectively, those categories indicate a risk from 9-18%, moderate risk levels.

- IncomeRange: most income range for prosper loans beneficial had from 25000 to 49999 dollars.

- BorrowerState: CA is the top state of borrowing prosper loans among all the state followed by TX, NY, and FL with a slight difference among them.

- Occupation: the result was irrelevant, no need to further investigating this feature.

- InterestRate: the distribution seems bimodal, since it has two peaks. Also, a major lack of fit exists on the right side of the observed distribution where the second peak appears.

- Term: most loans have a 3 years period.

- MonthlyLoanPayment: most borrowers pay 137.71 dollars per month.

### Key Insights for Presentation
Most of the features above will be represented in the presentation except Occupation, Term, IncomeRange and MonthlyLoanPayment. 

### Bivariate Exploration
- ProsperRatingAlpha vs LoanStatus: most of the current loans were under C, B, and A respectively moderate risk levels while most completed loans fill under D risk category. The graph also indicates that a little amount of current and completed loans were under AA (lower risk) risk category only. This an interesting relationship as almost a significant amount of prosper's loan borrowers tend to take moderate to higher level category risk.

- CreditGrade vs LoanOriginalAmount: A very interesting relation represented, the graph shows the distribution shape of all credit grade compared to loan original amount. Almost credit grade AA, A, B, C, and D had the largest values and reasonable distribution shape. According to the loan original amount values, the median of credit grade A was the largest followed by B then AA respectively. This correlation indicates that as credit grade get higher as the original amount of loans increases.

- CreditGrade vs Term: a great portion of C credit grade owners tend to have a 3 years period loan. Since there is no relevant relation indicated no need to investigate it more.

- Term vs InterestRate: the higher median of interest rate was represented in the 5 years term loans which approximately reach a 0.19. Also, the lowest median was associated with one-year term loans as expected. The distribution indicates that the most contributed loans were 3 years term period with a median of interest rate equal to 0.17 approximately. As represented, loans taken by one year period have less interest rates than the longer term loans.

- BorrowerAPR vs CreditGrade: a strong correlation was indicated between ARP rate and credit grade. As the credit grades get higher as the ARP rates get lower.

- InterestRate vs CreditGrade: As expected as the credit grade increases as the interest rate decrease. A strong correlation indicated.

- LoanOriginalAmount vs MonthlyLoanPayment: the plot has a healthy trend line for the mean of both variables, the monthly payment amount increases as the amount of the orignal loan get higher. To resolve the higher monthly payment amount, first borrower has to minimize the amount of original loan amount; secondly, they should extend the term of the loan for example from 3 years to 5.

### Key Insights for Presentation
All the insights will be represented excluding BorrowerAPR vs CreditGrade, LoanOriginalAmount vs MonthlyLoanPayment and CreditGrade vs Term relation graph.

### Multivariate Exploration

- LoanOriginalAmount vs MonthlyLoanPayment vs Term: almost all the one year borrowers tend to pay there monthly amount comparing with the other terms. Also, as the higher number of users tend to have three years period term they don't show commitment to pay their monthly portion. To resolve this issue, the borrowers who struggle with their monthly payment rate should extend the term from 3 years to 5 years and borrow a lesser amount of loan.

- BorrowerAPR vs InterestRate vs ProsperRatingNumeric: a strong correlation between APR, interest rate and prosper rating of the risk was represented. As the prosper rating gets higher as both APR & interest rate get lower.

- LoanOriginationQuarter vs InterestRate vs Term: for one-year term loans specifically in Q4 of 2010, the interest rate was the lowest, While in Q2 and Q3 of 2011 was the highest. Moreover while reading the three years term interest rate, almost all rates have a fixed interest rate amount between 0.14 - 0.24 distributed among all quarters; while the lowest was in Q4 of 2005 which was equal to 0.089. Moving to the five years term, the interest rate doesn't have a fixed range but the lowest was in Q4 of 2010. To conclude the 1 year period loan had the lowest interest rate among all quarters as shown in the above graph.

### Key Insights for Presentation
All investigated insight above will be represented in the presentation.


### Resources:
- https://www.udacity.com/
- https://en.wikipedia.org/wiki/Prosper_Marketplace
- https://www.lendingmemo.com/risk-grades-lending-club-prosper/
- https://help.lendingclub.com/hc/en-us/articles/216127747-What-is-the-difference-between-a-loan-that-is-in-default-and-a-loan-that-has-been-charged-off-
- https://robertmitchellv.com/blog-bar-chart-annotations-pandas-mpl.html
- https://matplotlib.org/api/text_api.html?highlight=get_text#matplotlib.text.Text
- https://datavizcatalogue.com/methods/violin_plot.html
