# Prosper Loan Data Exploration Analysis
## by  Uma Maheswari Raju


## Dataset

> Prosper was founded in 2005 as the first peer-to-peer lending marketplace in the United States. Since then, Prosper has facilitated more than $13 billion in loans to more than 860,000 people. Prosper Marketplace is backed by leading investors including Sequoia Capital, Francisco Partners, Institutional Venture Partners, and Credit Suisse NEXT Fund. In this Exploratory Data Analysis, I explore a Prosper dataset containing loan information for over a 100,000 people between the years 2006 and 2013.

> This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. 

> This project is divided into three parts such as Univariate plots, Bivariate PLots and Multivariate PLots and Summary Plots which summarize the final outputs of this exploratory analyses

### Data
> The data is available in the CSV format and can be downloaded from Here. A detailed information of the variables is mentioned Here

### Variables Explored
> Term : Amount of month customers opted for loan

> LoanStatus : Current status of the loan like chargedoff, completed, defauted etc...

> EstimatedEffectiveYield : Yield of lenders from borrowers minus the processing fee and late fines

> ProsperScore : Risk Factor score from 1 to 10. 10 being least risky

> BorrowerAPR : The Borrower's Annual Percentage Rate (APR) for the loan.

> BorrowerRate : The Borrower's interest rate for this loan.

> ListingCategory..numeric. : Prosper rating for borrowers in numbers

> EmploymentStatus : Current type of employment

> Occupation : Occupation of borrower at the time of listing

> EmploymentStatusDuration : How long the employee has been employed

> IsBorrowerHomeowner : Does the borrower owns house at the time of listing (True & False)

> ProsperRating..Alpha. : Prosper rating for borrowers in alphabets

> IncomeVerifiable : If the income of the borrower is verifiable at the time of listing (True & False)

> StatedMonthlyIncome : Monthly income of the borrower

> MonthlyLoanPayment : Monthly loan payment amount

> Recommendations : Recommendations the borrowers has at the time of listing

> DebtToIncomeRatio : The debt to income ratio of the borrower at the time the credit profile was pulled.

> LoanOriginalAmount : Original amount of the loan

> LoanOriginationQuarter : Quarter of the month when loan was originated


## Summary of Findings

> The prospser loans dataset contains over 100k observations with 81 variables distributing across 9 years. INitially,  understanding the variables, terminology and general domain knowledge of financial peer-to-peer lending was the first obstacle in approaching this dataset. Another hurdle was which variable to consider for the analyses, not drifting too far off any one path of investigation and not pulling in new variables throughout the process. Below are key insights found through this analysis:

- It’s very clear that as we go down the ladder of risk - from a ‘High Risk’ to an ‘AA’ rating - the APR for the borrower reduces drastically. 

- The variation in APRs also decreases as the loans get less riskier as displayed by the decreasing size of the boxes in the boxplots when going from ‘HR’ to ‘AA’. 

- We can clearly observe that for both BorrowerAPR and BorrowerRate which are metric for interest rates, we see a declining trend as the ProsperScore is increasing. This justifies the fact even more that lenders somehow prefers to charge less for all the borrowers with better ProsperScore as compared to borrowers with inferior ProsperScore.

- Here more score for the risk factor means better the borrower and lesser score for risk factor means poor prospects from the borrowers. We can see that for lower ProsperScore distribution of effective yield in a lot more than the higher ProsperScore. This may mean that lenders charges a variety of interest rate from the borrower with poor prospects as compared to borrowers with better prospect. We can also notice how median (represented by the black dot) is decreasing as ProsperScore is increasing. This may mean that lenders give more relaxations to borrowers with better ratings as compared to borrowers with poor rating.

- We can see from the above scatterplot that most of the MonthlyLoanPayment is distributed from 10 to 1000 and the StatedMonthlyIncome is distributed from 100 to 30000. There is definite a strong positive correlation between monthly income and monthly loan amount.

- We can see the positive linear relationship between loan original amount and monthly loan payment.

- It was interesting that ‘A’ category loans seem to have a lower APRs and a smaller range of debt-to-income ratios, both of which indicate less risk. The rest of the plot follow the color palette and APR increases as the rating gets riskier. Another thing is that most people tend to have debt-to-income ratios below 1, regardless of risk category. Lower ratings tend to be sparse in the 1.0+ debt-to-income ratio range.


## Key Insights for Presentation

>  The result shows loan origination year starts from 2005 to 2014 with number of listings. It indicates low listings during Q1 2006, Q4 2008 and Q3 2009. This time period coincides with the collapse of Lehman Brothers and the following fallout in the global financial system. Even though Prosper is an alternative to traditional loan models, it appears that its business was not immune to the global economic crisis. Perhaps Prosper’s credit policies were much looser before the credit crisis? After all, it appears that Prosper only established its Prosper Rating and Prosper Score in July 2009.

>  verall borrowers with better ratings tends to be less doubtful than borrowers with poor ratings. It means that the best borrowers are really best and the prosper rating really works.
Prosper rating with C has high number of listings(16.1%) and AA rating has low number of listings (4.7%). Both plots(prosper rating and creditgrade) is that there are less borrowers in the both ends of the credit rating (AA,HR,A,E). This is because most people with super good credit are financially stable and do not usually take loans while people at the tail-end of the credit rating don’t always get approved for credits.

> We can clearly observe that for both BorrowerAPR and BorrowerRate which are metric for interest rates, we see a declining trend as the ProsperScore is increasing. This justifies the fact even more that lenders somehow prefers to charge less for all the borrowers with better ProsperScore as compared to borrowers with inferior ProsperScore.

> We can see from the above scatterplot that most of the MonthlyLoanPayment is distributed from 10 to 1000 and the StatedMonthlyIncome is distributed from 100 to 30000. There is definite a strong positive correlation between monthly income and monthly loan amount.