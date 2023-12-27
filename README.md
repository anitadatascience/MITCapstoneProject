# MIT Data Science Capstone Project
MIT Data Science Capstone Project on Loan Default Prediction based on the domain

Problem Summary
—
Retail bank profits rely heavily on the interests they earn from home loans. The loans
are borrowed by regular income/high earning clients. But banks are also fearful for
defaulters as bad loans are a huge loss in profits so banks are judicious while approving
loans for their customer base. The approval loan process is extremely effort-intensive,
multifaceted, and prone to human error/biases.
Our objective is to build a machine that can learn this approval process and make it
more efficient and free of biases. The machine must not learn the same biases that
humans make. We need to build a classification model to predict clients who are likely
to default on their loan and give recommendations to the bank on the important features
to consider while approving a loan.

Proposed Solution
—
Based on the Home Equity dataset from the consumer’s credit department, we will build
a prediction model based on approved people with loans that either repaid or defaulted
on it. We will look at what key important factors to review when approving someone for
a loan.
There were various models that were tested and the best performing one was the tuned
random forest model.
Random forest is a type of decision tree model so it is easy to understand and easily
interpretable. It reduces the overfitting in decision trees through the method of taking
averages of multiple independent decision trees and there’s no need for pruning. At the
same time, it has all the pros in a decision tree which are less misclassification than
logistic regression, easy to visualize, mirrors human decision making more closely, and
requires little data preparation. It also outlines the important features we are looking to
review when approving a loan along with a high recall and precision score.

Data Exploration
—
We were provided the Home Equity dataset from the existing loan underwriting process
on recent applicants who had been approved for the credit.
The dataset contains the loan performance information for recent home equity loans on
5,960 clients. The loan defaulting occurred in 1,189 cases (20 percent). The target
(BAD) is a binary variable where 1 = “Client defaulted loan” and 0 = “loan repaid” along
with 12 other input variables regarding each applicant.
● BAD: 1 = Client defaulted on loan, 0 = loan repaid
● LOAN: Amount of loan approved.
● MORTDUE: Amount due on the existing mortgage.
● VALUE: Current value of the property.
● REASON: Reason for the loan request. (HomeImp = home improvement,
DebtCon= debt consolidation which means taking out a new loan to pay off other
liabilities and consumer debts)
● JOB: The type of job that loan applicant has such as manager, self, etc.
● YOJ: Years at present job.
● DEROG: Number of major derogatory reports (which indicates a serious
delinquency or late payments).
● DELINQ: Number of delinquent credit lines (a line of credit becomes delinquent
when a borrower does not make the minimum required payments 30 to 60 days
past the day on which the payments were due).
● CLAGE: Age of the oldest credit line in months.
● NINQ: Number of recent credit inquiries.
● CLNO: Number of existing credit lines. 
