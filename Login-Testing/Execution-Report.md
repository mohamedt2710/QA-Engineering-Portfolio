# Login Testing – Execution Report

## Execution Summary

| Metric | Result |
|---|---:|
| Total test cases | 5 |
| Executed | 5 |
| Passed | 5 |
| Failed | 0 |
| Not run | 0 |

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

## Conclusion
All five planned login test cases were executed successfully. No failures or defects were observed during this test session.

## Notes
Results are based on the manual execution observations reported during this test session.
