# Problems Faced and Solutions

> This file is a lab record template. The examples are common potential problems in reservation applications; they are not claims that these problems have already occurred. Keep only the issues you personally encounter and document the actual solution.

## Problem log

| No. | Problem / symptom | Possible cause | Suggested solution | Actual result in lab |
|---|---|---|---|---|
| 1 | GitHub push or authentication fails | Incorrect remote, credentials, or branch | Verify remote URL, sign-in/token permissions, and branch name | To be filled |
| 2 | User cannot register or sign in | Invalid input, validation, or authentication logic | Validate fields and inspect authentication errors; never store plain-text passwords | To be filled |
| 3 | Search returns no tickets | Incorrect filters or missing schedule data | Check input values, test data, and search conditions | To be filled |
| 4 | Selected seat/ticket becomes unavailable | Another booking changed availability | Recheck inventory at confirmation and prevent double booking in the data layer | To be filled |
| 5 | Total booking price is incorrect | Calculation or quantity error | Calculate from trusted price and quantity; test boundary cases | To be filled |
| 6 | Booking confirmation is not generated | Booking save or reference generation failure | Check persistence result and generate a unique reference after successful save | To be filled |
| 7 | Booking history shows incorrect records | User association or query filter error | Restrict the query to the authenticated user's ID and test access control | To be filled |
| 8 | Cancellation does not update booking status | Cancellation workflow or inventory update error | Define cancellation rules and update booking and availability consistently | To be filled |

## Detailed report format

Copy this section for every real problem:

### Problem [number] — [short title]
- **Date / lab session:**
- **Expected result:**
- **Actual result:**
- **Steps to reproduce:**
- **Error message / screenshot:**
- **Cause identified:**
- **Solution attempted:**
- **Retest result:**
- **Related GitHub issue or commit:**

## Notes
- Do not enter passwords, payment card numbers, or other sensitive information in this document.
- Use a payment sandbox or simulated payment for the laboratory prototype.
- If a problem remains unresolved, record it as unresolved and add the next action.
