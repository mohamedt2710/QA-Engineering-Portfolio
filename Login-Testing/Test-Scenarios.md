# Login – Test Scenarios

| Scenario ID | Scenario | Type | Priority |
|---|---|---|---|
| TS-LOGIN-001 | Verify login with valid username and password | Positive | High |
| TS-LOGIN-002 | Verify login with an invalid username | Negative | High |
| TS-LOGIN-003 | Verify login with an invalid password | Negative | High |
| TS-LOGIN-004 | Verify validation when both fields are empty | Negative | High |
| TS-LOGIN-005 | Verify validation when password is empty | Negative | Medium |
| TS-LOGIN-006 | Verify login behavior for a locked-out user | Negative | High |
| TS-LOGIN-007 | Verify username and password case sensitivity | Negative | Medium |
| TS-LOGIN-008 | Verify handling of leading/trailing spaces in credentials | Negative | Medium |
| TS-LOGIN-009 | Verify that the password field masks entered characters | UI | Medium |
| TS-LOGIN-010 | Verify login submission using the Enter key | Positive | Medium |
| TS-LOGIN-011 | Verify handling of very long username and password values | Boundary | Medium |

## Preconditions
1. The SauceDemo website is accessible.
2. A browser is available.
3. Use only the public demo credentials supplied by SauceDemo.

## General expected behavior
- Valid credentials should allow the user to reach the inventory/products page.
- Invalid or missing credentials should prevent login and show clear validation feedback.
- The application should not establish an authenticated session after a failed login.
- Password characters should be masked in the password input.
- Keyboard submission should behave consistently with clicking the Login button.

## Execution note
Scenario definitions do not imply execution. Check the corresponding test case status and execution report for verified results.
