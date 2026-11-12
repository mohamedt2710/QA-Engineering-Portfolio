# Login Testing – Execution Report

## Execution Summary

| Metric | Result |
|---|---:|
| Total test cases | 5 |
| Executed | 4 |
| Passed | 4 |
| Failed | 0 |
| Not run | 1 |

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

## Pending Test Case
- TC-LOGIN-005 – Submit username without password

## Notes
Only the four test cases above were executed and confirmed during this test session. The remaining case is intentionally marked as **Not Run**. No defects have been reported because no unexpected behavior has been observed so far.
