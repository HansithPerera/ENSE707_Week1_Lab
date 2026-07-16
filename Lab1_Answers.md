\# ENSE707 Week 1 Lab - Answers



\## Activity 1



\### 1. Why does regular committing support software quality?



Regular committing keeps changes small and isolated, which makes 

defects easier to find and fix (supporting early defect detection 

and Boehm's First Law). It enables Continuous Integration, because 

CI only works when developers commit frequently so automated builds 

and tests can catch problems early. Small commits also support 

prevention over correction, improve maintainability (clear history, 

easy revert), and make code review practical. Without regular 

commits, modern quality practices like CI/CD, shift-left testing, 

and peer review break down.



\### 2. How can Git history provide evidence of individual progress?



\- \*\*Attribution\*\* — every commit is tagged with the author's name, 

&#x20; proving individual contribution vs. teammates

\- \*\*Timeline\*\* — timestamps show consistent effort over time

\- \*\*Volume\*\* — `git shortlog -sn` quantifies commits and lines contributed

\- \*\*Skill growth\*\* — early vs. later commits show improvement

\- \*\*Problem-solving\*\* — commit messages document what was fixed and how

\- \*\*Iteration\*\* — history reveals drafts, refactors, and revisions

\- \*\*Workflow discipline\*\* — branches, PRs, and reviews show 

&#x20; professional habits

\- \*\*Responsiveness\*\* — post-review commits show acting on feedback

\- \*\*Ownership\*\* — `git blame` shows which parts of the code you authored



\## Activity 3

\### 1. What happens if the opening balance is negative?

The account is created with a negative balance, no validation prevent it. an account with negative balance with negative 

opening balance makes no business sense. We can come to the conclusion that the customer owes money before doing anything.


\### 2. What happens if a deposit amount is negative?

Negative deposit would substract from the balance, effectively acting as an unauthorised withdrawal. 

This could lead to incorrect account balances and potential overdraft situations, which is not a valid operation in banking systems.

Therefore, deposits should always be validated to ensure they are positive amounts.


\### 3. What happens if a withdrawal amount is greater than the balance?

The balance goes negativea and overdrawn, and according to the code it returns true, even though the account is overdrawn. 

This is not a valid operation in banking systems and should be fixed, as it allows the account to go into debt without proper authorization or overdraft protection.


\### 4. Is the transaction fee calculation clearly documented?

No, the 0.02m is just a random number as it seems like, with no comment or explanation. It is not clear how the fee is calculated, 

and it should be documented to ensure transparency and understanding of the fee structure.


\### 5.  Is the class easy to test?

The methods are public and return values that can be asserted against, so yes, the class is easy to test. However, 

the lack of validation for negative deposits and withdrawals makes it harder to test edge cases and error handling.


\### 6. What functional requirements are missing?

A bank needs create accounts, deposit money, withdraw money, prevent overdrafts, calculate fees, provide account statements
display balance, and handle errors. The current implementation is missing validation for negative deposits and withdrawals.

\### 7.What non-functional quality attributes are relevant?

- **Reliability** — the system should consistently perform as expected without failures.
- **Maintainability** — the code should be easy to understand, modify, and extend.
- **Performance** — the system should handle transactions efficiently, even under load.
- **Security** — sensitive financial data must be protected against unauthorized access.


## Activity 4 - QA vs QC

QA abd QC are both essential to software quality but operate at differently.
**Quality Assurance(QA** is process oriented and proactive. It focuses on preventing defects before they occur by improving the processes used to develop the software.
Rahther than checking whether a specific product is correct, QA asks whether the team is following the practices that consistently produce correct products. with examples like
coding standards reviewing requirements,a auditing processes and training the team. the philosophy is buid quality into the process rather than inspect it inot the product.

**Quality Control(QC)** is product oriented and reactive. it focuses on identifying defects in actual software after the development processes. QC asks direct question that if the build meet
it's specified requirements? this includes unit testing, executing acceptance tests, and reporting defects. QC is reactive because it identifies defects that already exist.

**Key differences between QA and QC:**

| Aspect | Quality Assurance (QA) | Quality Control (QC) |
|--------|-----------------------|---------------------|
| Focus | Process-oriented, proactive | Product-oriented, reactive |
| Timing | Throughout development | After development exist |
| Approach | Prevents defects | Identifies defects |

### Classification of activities

Writing coding standards for money calculations  - QA
Running unit tests for withdrawal behaviour - QC
Reviewing requirements for ambiguity - QA
Testing negative deposit input - QC
Analysing repeated transaction defects - QC
Reporting a failed test case - QC
Creating a checklist for financial validation rules - QA
Retesting after fixing withdrawal logic - QC


