# Login – Test Scenarios

| Scenario ID | Scenario | Type | Priority |
|---|---|---|---|
| TS-LOGIN-001 | Verify login with valid username and password | Positive | High |
| TS-LOGIN-002 | Verify login with an invalid username | Negative | High |
| TS-LOGIN-003 | Verify login with an invalid password | Negative | High |
| TS-LOGIN-004 | Verify validation when both fields are empty | Negative | High |
| TS-LOGIN-005 | Verify validation when password is empty | Negative | Medium |

## Preconditions
1. The SauceDemo website is accessible.
2. A browser is available.
3. Use only the public demo credentials supplied by SauceDemo.

## General expected behavior
- Valid credentials should allow the user to reach the inventory/products page.
- Invalid or missing credentials should prevent login and show a clear validation message.
- The application should not expose a successful authenticated session after a failed login.
