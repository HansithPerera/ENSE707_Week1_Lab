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

