# Prosper Loan Dataset

## by Uju Chinedum

## Dataset

> The dataset comprises of 113937 rows and 81 columns initially with 3 boolean columns, 61 numeric columns and 14 object columns but there are a lot of columns with too many missing values and incorrect data types. After investigatig those columns, I found that they were unique and needed but with no way to get them, I decided to drop those columns with extreme missing values (i.e >=58848 missing values) and fill the remaining. After that the new dataframe comprised of 113937 rows ands 69 columns with 3 boolean columns, 4 datetime columns, 48 numeric columns and 14 object columns.

## Summary of Findings

> - The distribution of BorrowerAPR looks normal but with a spike in value at around 0.35 - 0.37
> - From the visualizations above, I observed that the ProsperRating (numeric) and ProsperRating (Alpha) are infact the same and the only difference was how they were represented. The frquency of these two increased as the ratings until they got to the modal rating and then began to fall. ProsperScore observed a similar pattern.
> - The distribution of EmploymentStatus showed that Employed people tend to apply for loan more than others. It may be argued that this is because the missing values of those features were filled with their mode but that just implies that they were alreadng leading results in said features
> - The distribution of LoanOriginalAmount is not skewed. Even with a log transformation, there is no change. But most people had an origination amount of about 4000 - 5000
> - While the distribution of TotalTrades was skewed to the right, it still showed that most people tended to have trade lines of between 20 - 25.
> - A closer look at the distribution of MonthlyLoanPayment showed that most people were expected to pay around 160 - 230 dollars.
> - The relationship between the Prosper Score and Income Verifiable shows that verification of income plays an important role in the Prosper Score. Prosper Score 10 and 11, which are the highest, are only applied to those who have verifiable sources of income. But Prosper Score 5, which is the modal Score, has the most people with verified sources of income.
> - The relationship between the Numeric Prosper Rating and Prosper Score against Employment Status. It shows that for every Rating and Score, Employed people made up most of the consideration. Not available and Part-time made up the least except in the Rating 4 and Score 5 where Full-time makes the highest consideration and Not available also made a considerable portion compared to others.
> - The relationship between the Prosper Score and Borrower APR that Prosper Score 5 had a wider range of Borrower APR and the lowest Borrower APR of all the Score. Prosper Score 4 had the highest Borrower APR. Though there were a lot of outliers in Prosper Score 1 and it also had the lowest range of Borrower APR.
> - The distribution of Monthly Loan Payment for each Alphabetic Prosper Rating that Rating C had the most occurence of Monthly Loan Payment.
> - The relationship between the Total Trades and Current Credit Lines, Open Credit Lines and Total Credit Lines In The Past 7 Years. It shows that they are all positively correlated with Total Credit Lines In The Past 7 Years having the highest correlation.
> - The relationship between Prosper Rating and Prosper Score. Each Rating had varying levels of Score but Rating 5 had the highest Score of 4. I also noticed that Scores 8, 9, 10, 11 had no relationhip with the Ratings.

## Key Insights for Presentation

> - What is the relationship between `ProsperScore` and `ProsperRating`?
> - Does `ProsperScore` influence `BorrowerAPR`?