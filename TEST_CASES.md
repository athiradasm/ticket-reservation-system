# Test Cases — Ticket Reservation System

**Project:** Ticket Reservation System  
**Repository:** https://github.com/athiradasm/ticket-reservation-system  
**Document purpose:** Test cases for the project work recorded in this GitHub repository.

> **Execution note:** These are prepared test cases, not test results. The reservation application has not yet been implemented, so application test cases are marked **Not Run**. Execute them after implementation and record the actual result and evidence. Repository/documentation checks can be performed now.

## 1. Test cases for GitHub repository and project documentation

| Test ID | Test scenario | Test steps | Expected result | Actual result | Status |
|---|---|---|---|---|---|
| GH-01 | Open the project repository | Open the repository URL in a browser | Repository page loads and displays the project | To be recorded | Not Run |
| GH-02 | Verify project README | Open README.md | Project title, description, aim and objectives are visible | To be recorded | Not Run |
| GH-03 | Verify storyboard document | Open STORYBOARD.md | Six screens and the user flow are documented | To be recorded | Not Run |
| GH-04 | Verify progress tracker | Open PROGRESS.md | Session-wise progress table and task statuses are visible | To be recorded | Not Run |
| GH-05 | Verify problems document | Open PROBLEMS.md | Problem log and detailed report template are visible | To be recorded | Not Run |
| GH-06 | Verify development issues | Open the repository Issues page | Project tasks are listed as GitHub issues | To be recorded | Not Run |

## 2. Functional test cases for the proposed reservation system

| Test ID | Module | Test scenario / input | Expected result | Actual result | Status |
|---|---|---|---|---|---|
| TC-01 | Registration | Submit registration with all valid required details | Account is created and a success message is shown | To be recorded | Not Run |
| TC-02 | Registration | Submit registration with a required field empty | Validation message is shown; account is not created | To be recorded | Not Run |
| TC-03 | Registration | Register with an email/username already in use | Duplicate account is rejected with a clear message | To be recorded | Not Run |
| TC-04 | Login | Enter valid registered credentials | User is authenticated and taken to the appropriate page | To be recorded | Not Run |
| TC-05 | Login | Enter an incorrect password | Login is rejected without exposing sensitive information | To be recorded | Not Run |
| TC-06 | Ticket search | Search using valid criteria and a future date | Matching available services/tickets are displayed | To be recorded | Not Run |
| TC-07 | Ticket search | Search with no matching service | A “no results” message is shown; user can search again | To be recorded | Not Run |
| TC-08 | Ticket search | Submit search with required criteria missing | Input validation is shown and search is not processed | To be recorded | Not Run |
| TC-09 | Availability | View a service with available tickets/seats | Correct availability and ticket details are displayed | To be recorded | Not Run |
| TC-10 | Selection | Select an available seat or valid ticket quantity | Selection is accepted and summary is updated | To be recorded | Not Run |
| TC-11 | Selection | Attempt to select an unavailable seat or excess quantity | Selection is rejected and availability is explained | To be recorded | Not Run |
| TC-12 | Price calculation | Select multiple tickets | Total equals ticket price multiplied by quantity, plus any clearly stated fees | To be recorded | Not Run |
| TC-13 | Booking review | Review booking before confirmation | Service, date, passenger/seat details and total are correct | To be recorded | Not Run |
| TC-14 | Booking | Confirm a valid booking while tickets remain available | Booking is saved and a unique booking reference is generated | To be recorded | Not Run |
| TC-15 | Booking conflict | Two users attempt to reserve the same final seat/ticket | Only one reservation succeeds; duplicate booking is prevented | To be recorded | Not Run |
| TC-16 | Payment/demo step | Simulate an approved payment success | Booking is confirmed only after successful simulated payment | To be recorded | Not Run |
| TC-17 | Payment/demo step | Simulate payment failure or cancellation | Booking is not incorrectly marked as paid/confirmed; clear message is shown | To be recorded | Not Run |
| TC-18 | Confirmation | Open confirmation after successful booking | Correct booking reference and reservation details are displayed | To be recorded | Not Run |
| TC-19 | Booking history | Open My Bookings as a signed-in user | Only that user's reservations are displayed | To be recorded | Not Run |
| TC-20 | Access control | Attempt to view another user's booking | Access is denied; private booking details are not disclosed | To be recorded | Not Run |
| TC-21 | Cancellation | Cancel a booking that is eligible for cancellation | Booking status changes to cancelled and availability is updated according to rules | To be recorded | Not Run |
| TC-22 | Cancellation | Attempt cancellation after the allowed cancellation period | Cancellation is refused with an explanatory message | To be recorded | Not Run |
| TC-23 | Input/security | Enter unexpected text or script-like input in form fields | Input is safely validated/handled; application does not execute injected content | To be recorded | Not Run |
| TC-24 | Session/logout | Log out and try to open a protected booking page | User is logged out and redirected to login or denied access | To be recorded | Not Run |

## 3. Test execution summary

Fill this table after running the tests. Do not count a test as passed until its actual result has been checked.

| Category | Total prepared | Passed | Failed | Not Run |
|---|---:|---:|---:|---:|
| GitHub/documentation checks | 6 | 0 | 0 | 6 |
| Reservation system functional tests | 24 | 0 | 0 | 24 |
| **Total** | **30** | **0** | **0** | **30** |

## 4. Test execution record

For each test, update the Actual result and Status columns above. Use **Passed**, **Failed**, or **Blocked**. If a test fails, record the observed error, steps to reproduce, screenshot/evidence, and issue number below.

### Defect report template
- **Test ID:**
- **Date tested:**
- **Environment / browser / device:**
- **Steps to reproduce:**
- **Expected result:**
- **Actual result:**
- **Evidence / screenshot:**
- **GitHub issue created:**
- **Retest result:**

## 5. Assumptions to confirm before execution

- Confirm whether the system reserves bus, train, movie, or other event tickets.
- Confirm the required fields and booking rules from the laboratory assignment.
- Confirm the selected programming language, framework, and database.
- Use simulated payment or an approved sandbox for testing; do not enter real card details.
- Adjust test cases to match the final implemented requirements.
