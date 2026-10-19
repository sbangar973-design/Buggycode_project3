# Buggycode_project3
# Student Utils – Unit Testing

## Project Overview
`student_utils.py` contains utility functions for calculating students' average marks, checking whether a student has passed, and assigning grades based on average marks.

## Functions
- `calculate_average(marks)`: Calculates the average of the given marks.
- `is_passing(mark)`: Checks whether a student has passed. The passing mark is 40.
- `get_grade(average)`: Assigns a grade based on the student's average:
  - 90 and above: Distinction
  - 60–89: First
  - 45–59: Second
  - Below 45: Fail

## How to Run the Tests
Run the following command in your terminal:

```bash
python test_student_utils.py
```

## Testing Results
- **Total tests:** 9
- **Final result:** All 9 tests passing
- **Status:** GREEN

## RED → FIX → GREEN

1. **RED:** Initially, tests identified errors in the implementation, including incorrect average calculation and boundary conditions.
2. **FIX:** Corrected the average calculation, passing-mark condition, and grade-checking order.
3. **GREEN:** Ran the test suite again and verified that all 9 tests passed successfully.

## Conclusion
The utility functions were corrected and verified using Python's `unittest` framework. All nine test cases passed, confirming the expected behavior for the tested inputs.
