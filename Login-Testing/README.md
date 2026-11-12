# Project 01 – SauceDemo Login Testing

## Project Overview
Manual testing of the login functionality of SauceDemo (Swag Labs), a public e-commerce demo application.

- **Application:** SauceDemo
- **URL:** https://www.saucedemo.com/
- **Testing type:** Manual functional testing
- **Test environment:** Web browser

## Objective
Verify that the login feature handles valid credentials, invalid credentials, and missing input correctly, and that users receive clear validation feedback.

## Scope
The initial execution covered:
- Successful login with valid credentials
- Invalid username
- Invalid password
- Empty username and password
- Username provided without password

The test inventory has now been expanded with additional scenarios for locked-out users, credential case sensitivity, whitespace, password masking, Enter-key submission, and long input values. These six additional cases are marked **Not Run** until they are executed and verified.

## Test Approach
Test cases are designed from the login flow and executed manually. Actual results and statuses are recorded after execution. A defect is reported only when the observed behavior differs from the expected behavior and the issue can be reproduced.

## Execution Summary

| Metric | Result |
|---|---:|
| Total test cases in inventory | 11 |
| Executed | 5 |
| Passed | 5 |
| Failed | 0 |
| Not run | 6 |
| Pass rate (executed cases) | 100% |

## Findings
- Valid demo credentials successfully redirected the user to the inventory page.
- Invalid credentials were rejected with an authentication error message.
- Empty and incomplete login submissions were rejected with validation messages.
- No defects were observed in the five executed test cases.

See the [Execution Report](Execution-Report.md) for test data, expected results, actual results, and individual statuses.

## Project Files
- [Test Scenarios](Test-Scenarios.md)
- [Test Cases](Test-Cases.csv)
- [Execution Report](Execution-Report.md)
- [Bug Report Template](Bug-Report-Template.md)

## Test Data
Use only the public demo credentials documented by SauceDemo. Never use personal or real account credentials.

---
**Project 01** – Part of the QA Engineering Portfolio.
