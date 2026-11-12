# Project 02 – Registration Functionality Testing

## Objective
Practice manual testing of a registration form, including successful registration, required fields, password confirmation, and username validation rules.

## Application Under Test
- Name: Expand Testing – Register
- URL: https://practice.expandtesting.com/register
- Type: Public practice web application

## Scope
- Register with valid data
- Attempt registration with an existing username
- Password and confirmation mismatch
- Empty registration form and missing confirmation
- Username format, length, spaces, and hyphen-position validation

## Test approach
All recorded tests were executed manually in a browser. Actual results below are based on the observed messages reported during execution. A test is marked PASS only when the observed behavior matches the expected behavior.

## Test data
Use the sample values documented in the test cases. These are practice credentials only; do not reuse real passwords.

## Project files
- [Test Scenarios](Test-Scenarios.md)
- [Test Cases](Test-Cases.csv)
- [Execution Report](Execution-Report.md)
- [Bug Report Template](Bug-Report-Template.md)

## Execution summary
- Total executed: 11
- Passed: 10
- Needs investigation: 1
- Failed: 0 confirmed
- Not run: 0

The existing-username test returned a generic registration error. This does not confirm the exact cause, so it is kept as Needs Investigation rather than reported as a confirmed defect.

## Learning outcomes
- Design positive and negative registration tests
- Validate required fields and input rules
- Record actual results accurately
- Distinguish an unexpected result from a confirmed defect
