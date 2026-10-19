
# Audit Report: Student Utils

## 1. Project Overview
The Student Utils project contains Python functions for calculating average marks, checking passing status, and assigning grades.

## 2. Files Audited
- `student_utils.py`
- `test_student_utils.py`
- `README.md`

## 3. Audit Findings

### Issue 1: Incorrect Average Calculation
- **Problem:** The average was calculated using `len(marks) - 1`.
- **Fix:** Changed the divisor to `len(marks)`.

### Issue 2: Passing Mark Boundary
- **Problem:** A mark of 40 was not considered passing.
- **Fix:** Changed the condition from `>` to `>=`.

### Issue 3: Grade Checking Order
- **Problem:** The Distinction condition was placed after the First-grade condition.
- **Fix:** Checked the highest grade first.

## 4. Testing
- **Framework:** Python `unittest`
- **Total test cases:** 9
- **Expected result:** All 9 tests pass.
- **Final status:** GREEN, after successful execution of all tests.

## 5. RED → FIX → GREEN

- **RED:** Initial tests identified errors in the program logic.
- **FIX:** Corrected the average calculation, passing boundary, and grade-checking order.
- **GREEN:** Reran the tests to verify the corrections.

## 6. Conclusion
The identified issues were corrected, and the program was tested using nine unit tests. The project is considered successful when all nine tests pass.

**Test command:**
```bash
python test_student_utils.py
```
