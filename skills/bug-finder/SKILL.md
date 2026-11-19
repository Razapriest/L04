


---
name: bug-finder
description: Find bugs in Python exercise files and save structured reports.
---

Analyze the provided Python file with line numbers.

Find every bug by comparing the implementation with its docstring.

For each bug, output exactly this format:

Line: [line number]
Problem: [what is wrong and why]
Example: [actual result versus expected result]
Fix: [correct Python code]

Write one block per bug.
Do not include extra explanations.

Save the report in the reports directory.
The report filename must match the input Python filename.

For example:
- exercise1.py -> reports/exercise1.md
- exercise2.py -> reports/exercise2.md
- exercise3.py -> reports/exercise3.md
- exercise4.py -> reports/exercise4.md

Never hardcode a specific exercise number.
Create the reports directory if it does not exist.

