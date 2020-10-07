# data_visualization-_project
## (Loan Data from Prosper)
### Preliminary Wrangling
this data about banking loan in USA this data has 113,937 loans rows with 81 variables columns for each data record (loan), including loan amount, borrower rate (or interest rate) loan term , current loan status, borrower income, and many others


### What features in the dataset do you think will help support your investigation into your feature(s) of interest?

> The factors that have the most influence on predicting the outcome of a loan and therefore of most interest are:    
   >
   >+ Term (The length of the loan expressed in months)
   >+ ProsperScore (custom risk score)
   >+ EmploymentStatus (The employment status of the borrower)
   >+ MonthlyLoanPayment (The scheduled monthly loan payment)
   >+ BorrowerRate (The Borrower's interest rate for this loan)
   >+ LoanOriginalAmount (The origination amount of the loan)
   >+ OpenCreditLines (Number of open credit line)
   >+IncomeRange (how much maney this person get within a month)
   >+BorrowerState ( the place/ state where this person lives-in)
    Recommendations (Number of recommendations the borrower had at the time the listing was created)


the categorical columns are term , LoanStatus, ProsperRating (Alpha), ProsperScore, ListingCategory (numeric),BorrowerState,
Occupation, EmploymentStatus, IsBorrowerHomeowner, CurrentlyInGroup, IncomeRange, IncomeVerifiable,

the future of the intersinte are ListingNumber, ListingCreationDate, Term, LoanStatus, LoanOriginalAmount, BorrowerAPR, BorrowerRate, ListingCategory, BorrowerState, StatedMonthlyIncome, Occupation, EmploymentStatus, IsBorrowerHomeowner, CurrentlyInGroup, TotalInquiries, DebtToIncomeRatio, MonthlyLoanPayment, TotalTrades, Investors,IncomeRange,ProsperScore, OpenCreditLines
## Key Insights for Presentation

For the presentation, I answer below questions:

        What affects the borrower’s APR or interest rate?
        Are there differences between loans depending on how large the original loan amount was?

I start by introducing the Borrower Rate, Loan Original, and Prosper Score, followed by the Distribution of Prosper Score in different Employment Status and Income Ranges. Then dig more into the relationships between Borrower Rate and Loan Original Amount and I discovered how it could be affected by Income Ranges, Total Credit Lines-past7 years, and Income Range. Besides, I also presented the effect of Income Range on Prosper Score and Borrower Rate relationship.

    The most important finding is that the Loan Original Amount and Prosper Score significantly affect the Borrow Rate.

## Summary of Findings
Most of those who completed their loans has a ProsperScore above 3. Most of those who currently has loan, has a ProsperScore of 4, and the minimum count of loaners belong to those who has a ProsperScore of 1. The majority (~50,000) of people who currently has a loan are employed no matter what is their ProsperScore. If their ProsperScore is between 4 and 8, the population of employed loan borrowers in each particular ProsperScore is between 6000 and 8000. In ProsperScore of 2 to 8, the number of loaners who has a salary of 25-49k and 50-74k is more than others salary groups and if the ProsperScore is between 4 and 8, the population of both salaries of 25-49k and 50-74k groups ranges between 2500 and 3900. Plots also show that BorrowerRate has a negative relationship with LoanOriginalAmount and has a positive relationship with ProsperScore. IncomeRange also affect the LoanOriginalAmount in a positive way. The plot of the full data using a violin plot suggests that borrow rate is independant of income range and ranges ~0.15-0.21. TotalCreditLinespast7years does not play a significant role on controling the BorrowerRate and LoanOriginalAmount relationship. At each particular IncomeRange, by increasing the LoanOriginalAmount, the BorrowerRate decreases. Besides, apparently only those who has a IncomeRange above $100k, are borrowing higher LoanOriginalAmount (>$25000) and their BorrowerRate is <0.15. apparently, people with lower IncomeRange have higher BorrowerRate at each individual ProsperScore.

