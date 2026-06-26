# Sauce Demo Test Plan

**Project:** Manual QA Testing of Sauce Demo (Swag Labs)
**Tester:** Felicia Agbooluchi
**Date:** June 2026
**Version:** 1.0

---

## 1. Introduction

### Objective
Validate core functionality, negative paths, and edge cases of [saucedemo.com](https://www.saucedemo.com) — a demo e-commerce platform.

### Scope
The following areas are covered in this test plan:

- Login and session management
- Product listing and sorting
- Product details page
- Add/remove items from cart
- Checkout flow (information, overview, completion)
- Logout and navigation
- User type matrix (standard, locked_out, problem, performance_glitch, error, visual)

### Out of Scope

- Performance load testing
- Security penetration testing
- Payment gateway (simulated only)

---

## 2. Test Environment

| Component | Details |
|---|---|
| URL | https://www.saucedemo.com |
| Browser | Chrome v137.0.7151.79 |
| Device | iPhone XR (iOS 18.5) |
| Network | Stable internet |

---

## 3. Test Data

| Username | Password | Expected Behavior |
|---|---|---|
| standard_user | secret_sauce | All core flows work as expected. One defect found in checkout validation. |
| locked_out_user | secret_sauce | Login is blocked. User cannot access the application. |
| problem_user | secret_sauce | Image mismatches across product pages. 3 of 6 items cannot be added to cart. Last Name field blocks checkout. |
| performance_glitch_user | secret_sauce | Login succeeds but with extreme latency of 20-30 seconds. Checkout validation defect present. |
| error_user | secret_sauce | Missing product descriptions. 3 of 6 items cannot be added to cart. Last Name field non-functional. Finish button not clickable. |
| visual_user | secret_sauce | Image mismatches. Cart icon and checkout button misplaced. Price instability on inventory page. Sort filters broken. |

---

## 4. Entry and Exit Criteria

### Entry Criteria
- Test environment is accessible
- All credentials are valid and functional
- No blocking defects on login or critical path

### Exit Criteria
- All High priority tests executed with results documented
- Medium and Low tests executed with known issues logged
- At least one full regression run completed per user account

---

## 5. Testing Techniques Used

| Technique | Description |
|---|---|
| Positive testing | Verified all core flows work as expected for standard_user: login, browsing, sorting, add to cart, checkout, logout |
| Negative testing | Tested invalid inputs including empty fields, wrong passwords, special characters in name fields, alphabets in zip code |
| Error state testing | Verified correct error messages appear for locked_out_user and missing required checkout fields |
| Exploratory testing | Applied to problem_user, error_user, and visual_user to surface image mismatches, broken cart, non-functional fields, and UI misplacement |
| Cross-user testing | Applied the same core test case set independently to all 6 user accounts to identify account-specific defects |

---

## 6. Test Coverage

| Feature | Test Cases | Users Covered |
|---|---|---|
| Login | LOG-01, LOG-02, LOG-03, LOG-04 | All 6 users |
| Inventory and sorting | INV-01 to INV-07 | All 6 users |
| Cart | CRT-01 | All applicable users |
| Checkout | CHK-01 to CHK-05 | All applicable users |
| Navigation | NAV-01, NAV-02 | All applicable users |
| UI elements | EDGE-01, EDGE-02 | visual_user |

---

## 7. Deliverables

- Test plan (this document)
- Executed test cases ([TEST-CASES.md](./TEST-CASES.md))
- Bug reports ([bug-reports/README.md](./bug-reports/README.md))
- Bug report screenshots ([bug-reports/screenshots/](./bug-reports/screenshots/))
- Test execution summary (pass/fail per test case, included in TEST-CASES.md)

---

## 8. Test Execution Summary

| Status | Count |
|---|---|
| Pass | 65 |
| Fail | 19 |
| **Total** | **84** |
