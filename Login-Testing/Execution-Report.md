# Login Testing – Execution Report

## Execution Summary

| Metric | Result |
|---|---:|
| Total test cases in inventory | 11 |
| Executed | 5 |
| Passed | 5 |
| Failed | 0 |
| Not run | 6 |
| Pass rate (executed cases) | 100% |

> The pass rate is calculated from executed cases only. The six remaining cases are not included because they have not been executed.

## Executed Test Cases

### TC-LOGIN-001 – Login with valid credentials
- **Test data:** `standard_user` / `secret_sauce`
- **Expected result:** User is redirected to the inventory/products page.
- **Actual result:** User was redirected to the inventory page successfully.
- **Status:** PASS

### TC-LOGIN-002 – Login with invalid username
- **Test data:** `wrong_user` / `secret_sauce`
- **Expected result:** Login is rejected and a clear error message is displayed.
- **Actual result:** `Epic sadface: Username and password do not match any user in this service`
- **Status:** PASS

### TC-LOGIN-003 – Login with invalid password
- **Test data:** `standard_user` / `wrong_password`
- **Expected result:** Login is rejected and a clear error message is displayed.
- **Actual result:** `Epic sadface: Username and password do not match any user in this service`
- **Status:** PASS

### TC-LOGIN-004 – Submit both fields empty
- **Test data:** Empty username and empty password
- **Expected result:** Login is rejected and required-field validation is displayed.
- **Actual result:** `Epic sadface: Username is required`
- **Status:** PASS

### TC-LOGIN-005 – Submit username without password
- **Test data:** `standard_user` / empty password
- **Expected result:** Login is rejected and password-required validation is displayed.
- **Actual result:** `Password is required`
- **Status:** PASS

## Not Run – Pending Execution

| Test Case ID | Scenario |
|---|---|
| TC-LOGIN-006 | Login with locked-out user |
| TC-LOGIN-007 | Check credential case sensitivity |
| TC-LOGIN-008 | Check leading and trailing spaces |
| TC-LOGIN-009 | Verify password masking |
| TC-LOGIN-010 | Submit login using Enter key |
| TC-LOGIN-011 | Submit very long credential values |

These cases are documented in [Test-Cases.csv](Test-Cases.csv). Their actual results and statuses must be updated after manual execution.

## Conclusion

All five executed login test cases passed. Six additional cases remain pending. No failures or confirmed defects were observed in the executed test set.

## Execution Notes

- Results are based on the manual execution observations reported during the test session.
- The report does not claim that the six pending cases were tested.
- A defect should be reported only after an actual mismatch has been reproduced.
