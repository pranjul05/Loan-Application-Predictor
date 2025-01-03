# Loan-Application-Predictor
A loan application is used by borrowers to apply for a loan. Through the loan application, borrowers reveal key details about their finances to the lender. The loan application is crucial to determine whether the lender will grant the request for funds or credit. The data for training and testing has been taken from a CSV file that can be accessed using the link:

For training: "https://raw.githubusercontent.com/dphi-official/Datasets/master/Loan_Data/loan_train.csv".

For testing: "https://raw.githubusercontent.com/dphi-official/Datasets/master/Loan_Data/loan_test.csv"

The different types of variables in the dataset are Categorical, ordinal, and numerical.

-Categorical features: These features have categories (Gender, Married, Self_Employed, Credit_History, Loan_Status) -Ordinal features: Variables in categorical features having some order involved (Dependents, Education, Property_Area) -Numerical features: These features have numerical values (ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term)

These all features are analysed in detail using various plots to get insights.

After doing univariate analysis we concluded that:

-Applicants with high incomes should have more chances of loan approval. -Applicants who have repaid their previous debts should have higher chances of loan approval. -Loan approval should also depend on the loan amount. If the loan amount is less, the chances of loan approval should be high. -Lesser the amount to be paid monthly to repay the loan, the higher the chances of loan approval. Let's try to test the above-mentioned hypotheses using bivariate analysis

After looking at every variable individually in univariate analysis, we then explore them again with respect to the target variable.

Missing values are then analysed. There are missing values in Gender, Married, Dependents, Self_Employed, LoanAmount, Loan_Amount_Term and Credit_History features.

We treat the missing values in all the features one by one.

We can consider these methods to fill the missing values:

For numerical variables: imputation using mean or median For categorical variables: imputation using mode There are very less missing values in Gender, Married, Dependents, Credit_History and Self_Employed features so we can fill them using the mode of the features. In the Loan_Amount_Term we will replace the missing values using the mode of this variable. In the LoanAmount variable, the null values are replaced using the median value. After outlier treatment and some feature engineering, we build three different models for prediction and calculated its accuracy.

These come out as: -Logistic Regression: Mean Validation Accuracy 0.7800041228612657
