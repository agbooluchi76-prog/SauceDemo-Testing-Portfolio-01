# Sauce Demo Bug Reports

**Application:** [Sauce Demo](https://www.saucedemo.com)
**Tester:** Felicia Agbooluchi
**Testing Period:** June 2026
**Browser:** Chrome v137.0.7151.79
**Device:** iPhone XR (iOS 18.5)
**Total Bugs Found:** 19
**User Accounts Tested:** standard_user, locked_out_user, performance_glitch_user, problem_user, error_user, visual_user

---

## Bug Summary

| Bug ID | Title | User Account | Severity | Priority |
|---|---|---|---|---|
| [STAND-01](./STAND-01-special-chars-accepted-checkout.md) | Special characters accepted in name and zip code fields at checkout | standard_user | High | High |
| [LOCK-01](./LOCK-01-locked-out-user-login-error.md) | Login returns locked-out error message | locked_out_user | High | Low |
| [PERF-01](./PERF-01-login-delay-20-30-seconds.md) | Login delay of 20-30 seconds before inventory loads | performance_glitch_user | Medium | High |
| [PERF-02](./PERF-02-special-chars-accepted-checkout.md) | Special characters accepted in name and zip code fields at checkout | performance_glitch_user | High | High |
| [PROB-01](./PROB-01-image-mismatch-inventory-vs-detail.md) | Image mismatch between inventory page and product detail page | problem_user | Medium | Medium |
| [PROB-02](./PROB-02-3-of-6-items-cannot-add-to-cart.md) | 3 out of 6 items cannot be added to cart | problem_user | High | High |
| [PROB-03](./PROB-03-last-name-field-blocks-checkout.md) | Last name field not interactive; blocks checkout progression | problem_user | Critical | Critical |
| [ERR-01](./ERR-01-product-description-missing-detail-page.md) | Product detail page missing description | error_user | Medium | Medium |
| [ERR-02](./ERR-02-3-of-6-items-cannot-add-to-cart.md) | 3 out of 6 items cannot be added to cart | error_user | High | High |
| [ERR-03](./ERR-03-last-name-non-functional-allows-checkout.md) | Last name field non-functional but allows checkout to proceed | error_user | Critical | Critical |
| [ERR-04](./ERR-04-finish-button-not-clickable.md) | Finish button not clickable on order overview page | error_user | Critical | Critical |
| [ERR-05](./ERR-05-special-chars-accepted-checkout.md) | Special characters accepted in name and zip code fields at checkout | error_user | High | High |
| [VIS-01](./VIS-01-image-mismatch-inventory-vs-detail.md) | Image mismatch between inventory page and product detail page | visual_user | Low | Low |
| [VIS-02](./VIS-02-cart-icon-wrong-position.md) | Cart icon positioned incorrectly | visual_user | Medium | Medium |
| [VIS-03](./VIS-03-sort-low-to-high-not-working.md) | Sort filter Price (Low to High) does not sort correctly | visual_user | Medium | Medium |
| [VIS-04](./VIS-04-sort-high-to-low-not-working.md) | Sort filter Price (High to Low) does not sort correctly | visual_user | Medium | Medium |
| [VIS-05](./VIS-05-checkout-button-wrong-position.md) | Checkout button displayed at top instead of bottom | visual_user | Low | Low |
| [VIS-06](./VIS-06-inventory-price-does-not-match-cart-price.md) | Inventory page price does not match cart price; changes on every refresh | visual_user | High | High |
| [VIS-07](./VIS-07-special-chars-accepted-checkout.md) | Special characters accepted in name and zip code fields at checkout | visual_user | High | High |

---

## Severity Breakdown

| Severity | Count |
|---|---|
| Critical | 3 |
| High | 8 |
| Medium | 6 |
| Low | 2 |
