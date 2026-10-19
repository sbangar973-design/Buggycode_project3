# Buggycode_project3
# Student Utils – Unit Testing

## 1. Project Overview
The Student Utils project is a Python project that calculates student averages, checks passing status, and assigns grades. Python's `unittest` framework is used to test these functions.

## 2. Functions
- `calculate_average(marks)`: Calculates the average of the given marks.
- `is_passing(mark)`: Returns `True` if the mark is 40 or above; otherwise, returns `False`.
- `get_grade(average)`: Assigns a grade based on the average:
  - 90 and above: Distinction
  - 60–89: First
  - 45–59: Second
  - Below 45: Fail

## 3. Project Files
- `student_utils.py` – Contains the student utility functions.
- `test_student_utils.py` – Contains nine unit test cases.
- `README.md` – Provides project information and testing instructions.
- `audit.md` – Documents the audit findings, corrections, and RED → FIX → GREEN process.

## 4. How to Run the Tests
Run the following command in the terminal from the project directory:

```bash
python test_student_utils.py
```

## 5. Testing Summary
- **Testing framework:** Python `unittest`
- **Total test cases:** 9
- **Final result:** All nine tests should pass after the corrections.
- **Status:** GREEN when all tests pass successfully.

## 6. RED → FIX → GREEN

### RED
Initial testing identified errors in the program logic, including an incorrect average calculation, a passing-mark boundary issue, and an incorrect grade-checking order.

### FIX
The identified issues were corrected:
1. Changed the average divisor to `len(marks)`.
2. Changed the passing condition to `mark >= 40`.
3. Checked the Distinction condition before the First-grade condition.

### GREEN
The test suite is run again to verify the corrections. The project reaches the GREEN stage when all nine unit tests pass.

## 7. Audit Report
The `audit.md` file contains the audit summary, identified issues, corrections, testing details, and the RED → FIX → GREEN workflow.

## 8. Conclusion
This project demonstrates the use of Python functions, automated unit testing, and a systematic debugging process. The audit documents the issues and fixes, while the test suite verifies the expected behavior.


