# Registration Testing – Execution Report

## Summary

| Metric | Result |
|---|---:|
| Total test cases executed | 11 |
| Passed | 10 |
| Failed (confirmed) | 0 |
| Needs investigation | 1 |
| Not run | 0 |

## Execution details

| Test Case ID | Scenario | Status |
|---|---|---|
| TC-REG-001 | Register with valid data | PASS |
| TC-REG-002 | Register with existing username | NEEDS INVESTIGATION |
| TC-REG-003 | Password and confirmation mismatch | PASS |
| TC-REG-004 | All fields empty | PASS |
| TC-REG-005 | Confirmation password empty | PASS |
| TC-REG-006 | Invalid username format | PASS |
| TC-REG-007 | Username shorter than 3 characters | PASS |
| TC-REG-008 | Username starts with hyphen | PASS |
| TC-REG-009 | Username exceeds 39 characters | PASS |
| TC-REG-010 | Username ends with hyphen | PASS |
| TC-REG-011 | Username contains spaces | PASS |

## Observation requiring investigation

**TC-REG-002 – Existing username**

- First registration using `mohamedqa2026` succeeded.
- A second registration attempt using the same username returned: `An error occurred during registration. Please try again.`
- The response indicates that the second attempt did not complete successfully, but it does not clearly identify the cause.
- Further verification is required before classifying this as a confirmed defect.

## Conclusion

The registration form passed 10 of the 11 executed test cases. One case requires further investigation. No confirmed defects are reported in this execution cycle.

*Execution results are documented from the manual observations provided during the test session.*
