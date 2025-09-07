### Introduction
Even among approved borrowers, certain segments: low to mid income borrowers, short-term loans, debt consolidation or credit card loans, and high revolving credit users carry higher EMI stress and default risk.

Credit grades do not fully capture this vulnerability. Banks need a data driven approach to identify these at-risk borrowers, monitor their repayment behavior, and implement proper measures to reduce defaults.

### Dataset Columns

| Column Name          | Description                                           | Data Type   |
|---------------------|-------------------------------------------------------|------------|
| `id`                 | Unique loan record ID                                 | Integer    |
| `loan_amnt`          | Loan amount requested by the borrower                | Float      |
| `installment`        | Monthly EMI                                          | Float      |
| `term`               | Loan term (months)                                   | Integer    |
| `int_rate`           | Interest rate of the loan                            | Float      |
| `annual_inc`         | Borrower’s annual income                             | Float      |
| `dti`                | Debt-to-Income ratio                                 | Float      |
| `loan_status`        | Loan repayment status                                | String     |
| `emp_length`         | Years of employment                                  | String     |
| `emp_title`          | Job title                                            | String     |
| `purpose`            | Loan purpose                                         | String     |
| `issue_d`            | Loan issue date                                      | Date       |
| `grade`              | Credit grade assigned                                 | String     |
| `sub_grade`          | Credit sub-grade                                     | String     |
| `home_ownership`     | Home ownership type                                  | String     |
| `verification_status`| Income verification status                            | String     |
| `revol_util`         | Revolving credit utilization (%)                     | Float      |


### Borrower Characteristics and Risk Behavior
Low-income borrowers with large loans face the highest EMI stress, regardless of loan purpose or credit card usage. Moderate-risk borrowers, though few, carry high EMIs relative to income, making them early warning candidates. Banks should monitor EMI-to-Income ratios and risk segmentation to identify vulnerable borrowers.

### Loan Risk Analysis (High-Value Metrics)
Shorter-term loans increase EMI stress, while longer tenures ease repayment. Most moderate-risk borrowers fall in the 10–20% EMI-to-Income range. Credit grades (A–F) don’t fully capture stress; monitoring should include EMI-to-Income along with loan term and grade.

### Portfolio Stress Simulation
A 10% income drop and 2% interest rate hike shows low-to-mid income borrowers (<80k), short-term loans (36 months), and debt consolidation/credit card borrowers are most vulnerable. Even prime borrowers (A & B) experience stress, highlighting that credit grades may underestimate repayment risk under shocks.

### High-Risk Borrower Personas
Borrowers earning <20k are most at risk, especially renters and mortgage holders. Default risk decreases with income, but home ownership mainly matters at lower income levels. High revolving utilization predicts defaults more strongly than DTI. Banks should monitor low-income, high utilization borrowers closely.
