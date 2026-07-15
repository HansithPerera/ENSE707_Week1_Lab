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