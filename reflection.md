\# Reflection – Static Code Analysis



\### 1. What did you learn from this lab?



I learned that static code analysis tools can identify code quality, formatting, and security problems without executing the program. Pylint checks code quality, Flake8 checks style and formatting, and Bandit identifies common security risks.



\### 2. Which issue was the most important, and why?



The unsafe use of `subprocess` with `shell=True` was the most important issue because it can expose a program to command-injection risks. Removing unsafe subprocess usage improved the security of the application.



\### 3. How did the fixes affect the code quality?



I corrected the identified issues, improved naming and documentation, fixed formatting, and made file encoding explicit. The Pylint score improved from 4.80/10 to 10.00/10. Bandit reported no issues, and Flake8 reported no violations after the fixes.



\### 4. How will you use static analysis in future projects?



I will run static analysis tools during development and before submitting or deploying code. This will help me identify problems early, improve readability, and reduce common security risks.

