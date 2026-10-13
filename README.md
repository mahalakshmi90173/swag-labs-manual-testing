
# Swag Labs Manual Testing

Manual testing project for the **Swag Labs** demo e-commerce application: https://www.saucedemo.com/

## Objective
Verify the core user flow (login, products, cart and checkout start) using manually designed and executed test cases, and record any issues found.

## Scope: Modules Tested
| Module | Areas covered |
|---|---|
| Login | Valid login, invalid password, empty fields, empty password |
| Products | Product listing (names, images, prices, Add to Cart buttons) |
| Cart | Add product, remove product, continue shopping |
| Checkout | Open checkout information form, checkout with an empty cart |

## Test Summary
| Metric | Count |
|---|---|
| Total test cases | 11 |
| Pass (including reported) | 9 |
| Needs investigation | 1 |
| Not run | 1 |
| Confirmed defects | 0 |

**Open item:** `TC_CART_004` found that the checkout information form opens even when the cart is empty. This is logged as `INV-001` (under investigation). It is a potential issue, not a confirmed defect, until the expected behavior is confirmed. Follow-up test `TC_CART_005` is not yet run.

## Repository Contents
```
SwagLabs-Manual-Testing/
├── SwagLabs_Test_Cases.xlsx   # Test cases with steps, expected/actual results, status
└── SwagLabs_Defect_Log.xlsx   # Defect / investigation log
```

## Test Case Format
Each test case includes: Test Case ID, Module, Scenario, Preconditions, Steps, Test Data, Expected Result, Actual Result, Status, Defect ID.

## Approach
- Testing type: manual functional testing
- Techniques: positive and negative scenarios, input validation checks
- Tools: Microsoft Excel (test cases and defect log), web browser

## Next Steps
- Execute `TC_CART_005` and confirm the intended empty-cart behavior
- Add test cases for checkout completion, sorting/filtering, and logout
- Add screenshots as evidence

## Author
**Venkata Mahalakshmi Ayirravu**
