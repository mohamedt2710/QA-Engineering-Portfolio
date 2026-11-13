# E-Commerce Application Testing

## Project overview
A practical QA project focused on validating a sample e-commerce shopping journey on [SauceDemo](https://www.saucedemo.com/).

**Project type:** Manual web application testing  
**Application:** SauceDemo  
**Testing focus:** Authentication, product listing, cart management, checkout, and order confirmation  
**Execution status:** Test cases are documented; execution is pending. No pass/fail results or defects are claimed until the checks are performed.

## Objectives
- Validate the main customer purchase journey from login to order completion.
- Verify cart calculations and item consistency.
- Check required-field validation and negative scenarios.
- Identify usability and functional risks around checkout.

## Scope

### In scope
- Login with valid and invalid credentials
- Product inventory display and sorting
- Add/remove products from the cart
- Cart item details and navigation
- Checkout information validation
- Order overview and completion confirmation

### Out of scope
- Payment gateway processing (the demo application does not represent a real payment provider)
- Load, stress, and security testing
- Email/SMS notifications and real order fulfilment

## Test approach
1. Review the available application behavior and define test scenarios.
2. Prepare test data using the demo application's supported accounts.
3. Execute each test case manually and record actual results.
4. Report only reproducible defects with clear evidence.
5. Re-test fixes and run relevant regression checks.

## Test deliverables
| Artifact | Description |
|---|---|
| [Test Cases](test-cases.csv) | Structured functional test cases with execution status |
| [Bug Report Template](bug-report-template.md) | Consistent defect reporting format |

## Entry criteria
- Demo application is reachable.
- A supported test account is available.
- Test cases and expected results are reviewed.

## Exit criteria
- All planned cases have an execution result.
- Failed cases have linked, reproducible defect reports or a documented explanation.
- Critical purchase-flow checks have been reviewed.

## Risks and notes
- SauceDemo is a demonstration application; behavior and data may differ from production commerce systems.
- Test account behavior may be intentionally restricted depending on the selected account.
- Test results must include the execution date and account type used.

## Execution summary
**Not executed yet.** This is intentional: execution results will be added only after the tests are run and verified.

## Author
QA Engineering Portfolio — Mohamed Tantawy
