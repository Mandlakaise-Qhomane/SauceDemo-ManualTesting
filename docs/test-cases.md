# Comprehensive Manual Test Execution Matrix

**Project:** Sauce Demo Web Application Manual Testing Portfolio  
**Candidate:** Rethabile Cecil Mandlakaise Qhomane  
**Target URL:** `https://www.saucedemo.com/`  
**Document Version:** 1.0  

---

## Module 1: Authentication

### TC-001: Standard User Login
* **Test Case ID:** `TC-001`
* **Test Title:** Standard user login
* **Module:** Authentication
* **Objective:** Verify successful login using standard credentials.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: standard_user` | `Password: secret_sauce`
* **Execution Steps:**
  1. Navigate to `https://www.saucedemo.com/`.
  2. Enter `standard_user` into the username field.
  3. Enter `secret_sauce` into the password field.
  4. Tap the Login button.
* **Expected Result:** User is navigated to the Products inventory page.
* **Actual Result:** User was successfully navigated to the Products inventory page.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-001-standard-user-pass.png`

---

### TC-002: Locked Out User Login
* **Test Case ID:** `TC-002`
* **Test Title:** Locked out user login
* **Module:** Authentication
* **Objective:** Verify error handling when logging in with a locked-out account.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: locked_out_user` | `Password: secret_sauce`
* **Execution Steps:**
  1. Navigate to `https://www.saucedemo.com/`.
  2. Enter locked credentials (`locked_out_user` / `secret_sauce`).
  3. Tap the Login button.
* **Expected Result:** Login is blocked and an error message is displayed.
* **Actual Result:** Login was blocked with locked out error message.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-002-locked-user-pass.png`

---

### TC-003: Problem User Login
* **Test Case ID:** `TC-003`
* **Test Title:** Problem user login
* **Module:** Authentication
* **Objective:** Verify login behavior for problem user state.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: problem_user` | `Password: secret_sauce`
* **Execution Steps:**
  1. Navigate to `https://www.saucedemo.com/`.
  2. Enter credentials (`problem_user` / `secret_sauce`).
  3. Tap the Login button.
* **Expected Result:** User logs in with expected problem UI states.
* **Actual Result:** User logged in successfully with expected problem UI behaviors.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-003-problem-user-pass.png`

---

### TC-004: Performance Glitch User Login
* **Test Case ID:** `TC-004`
* **Test Title:** Performance glitch user login
* **Module:** Authentication
* **Objective:** Verify handling of simulated latency during login.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: performance_glitch_user` | `Password: secret_sauce`
* **Execution Steps:**
  1. Navigate to `https://www.saucedemo.com/`.
  2. Enter credentials (`performance_glitch_user` / `secret_sauce`).
  3. Tap the Login button.
* **Expected Result:** User logs in successfully after simulated delay.
* **Actual Result:** User logged in successfully following performance glitch delay.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-004-performance-user-pass.png`

---

### TC-005: Invalid Credentials Login
* **Test Case ID:** `TC-005`
* **Test Title:** Invalid credentials login
* **Module:** Authentication
* **Objective:** Verify error blocking for wrong password.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: standard_user` | `Password: wrong_password`
* **Execution Steps:**
  1. Navigate to `https://www.saucedemo.com/`.
  2. Enter invalid credentials (`standard_user` / `wrong_password`).
  3. Tap the Login button.
* **Expected Result:** Login is prevented and error message is displayed.
* **Actual Result:** Login was prevented and error message was displayed.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-005-invalid-login-pass.png`

---

## Module 2: Product Catalogue

### TC-006: View Product Details
* **Test Case ID:** `TC-006`
* **Test Title:** View product details
* **Module:** Product Catalogue
* **Objective:** Verify product detail page rendering.
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Product Name: Sauce Labs Backpack
* **Execution Steps:**
  1. Locate "Sauce Labs Backpack" on the inventory page.
  2. Tap the product title.
* **Expected Result:** User is navigated to product details page.
* **Actual Result:** User was successfully navigated to product details page.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-006-product-details-pass.png`

---

### TC-007: Sort Products by Price (Low to High)
* **Test Case ID:** `TC-007`
* **Test Title:** Sort products by price low-to-high
* **Module:** Product Catalogue
* **Objective:** Verify price sorting logic (ascending).
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Sort Option: Price (low to high)
* **Execution Steps:**
  1. Open the sort dropdown menu.
  2. Select "Price (low to high)".
* **Expected Result:** Products are re-ordered by price ascending.
* **Actual Result:** Products were successfully sorted by price ascending.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-007-sort-lohi-pass.png`

---

### TC-008: Sort Products by Price (High to Low)
* **Test Case ID:** `TC-008`
* **Test Title:** Sort products by price high-to-low
* **Module:** Product Catalogue
* **Objective:** Verify price sorting logic (descending).
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Sort Option: Price (high to low)
* **Execution Steps:**
  1. Open the sort dropdown menu.
  2. Select "Price (high to low)".
* **Expected Result:** Products are re-ordered by price descending.
* **Actual Result:** Products were successfully sorted by price descending.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-008-sort-hilo-pass.png`

---

### TC-009: Sort Products Alphabetically (A to Z)
* **Test Case ID:** `TC-009`
* **Test Title:** Sort products alphabetically (A to Z)
* **Module:** Product Catalogue
* **Objective:** Verify alphabetical sorting (A to Z).
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Sort Option: Name (A to Z)
* **Execution Steps:**
  1. Open the sort dropdown menu.
  2. Select "Name (A to Z)".
* **Expected Result:** Products are sorted alphabetically from A to Z.
* **Actual Result:** Products were successfully sorted from A to Z.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-009-sort-az-pass.png`

---

### TC-010: Sort Products Alphabetically (Z to A)
* **Test Case ID:** `TC-010`
* **Test Title:** Sort products alphabetically (Z to A)
* **Module:** Product Catalogue
* **Objective:** Verify reverse alphabetical sorting (Z to A).
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Sort Option: Name (Z to A)
* **Execution Steps:**
  1. Open the sort dropdown menu.
  2. Select "Name (Z to A)".
* **Expected Result:** Products are sorted alphabetically from Z to A.
* **Actual Result:** Products were successfully sorted from Z to A.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-010-sort-za-pass.png`

---

## Module 3: Cart

### TC-011: Add One Product to Cart
* **Test Case ID:** `TC-011`
* **Test Title:** Add one product to cart
* **Module:** Cart
* **Objective:** Verify successful item addition and cart badge update.
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Product Name: Sauce Labs Backpack
* **Execution Steps:**
  1. Tap "Add to cart" on the Sauce Labs Backpack item card.
* **Expected Result:** Button changes to "Remove" and cart badge updates to 1.
* **Actual Result:** Button changed to "Remove" and cart badge updated to 1.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-011-add-one-product-pass.png`

---

### TC-012: Add Multiple Products to Cart
* **Test Case ID:** `TC-012`
* **Test Title:** Add multiple products to cart
* **Module:** Cart
* **Objective:** Verify badge update and addition for multiple items.
* **Preconditions:** User is on the Products inventory page.
* **Test Data:** Multiple inventory items
* **Execution Steps:**
  1. Tap "Add to cart" on multiple distinct products in sequence.
* **Expected Result:** Cart badge reflects total count of added items.
* **Actual Result:** Cart badge accurately reflected total count of added items.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-012-add-multiple-products-pass.png`

---

### TC-013: Remove Product from Cart
* **Test Case ID:** `TC-013`
* **Test Title:** Remove product from cart
* **Module:** Cart
* **Objective:** Verify item removal and cart badge decrement.
* **Preconditions:** User has items in the cart.
* **Test Data:** N/A
* **Execution Steps:**
  1. Tap "Remove" button on an added product item.
* **Expected Result:** Item is removed and cart badge decrements accordingly.
* **Actual Result:** Item was removed and cart badge decremented accordingly.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-013-remove-product-pass.png`

---

### TC-014: Verify Cart Item Count
* **Test Case ID:** `TC-014`
* **Test Title:** Verify cart item count
* **Module:** Cart
* **Objective:** Verify that cart accurately displays item quantity.
* **Preconditions:** User has 1 product remaining in cart.
* **Test Data:** N/A
* **Execution Steps:**
  1. Open and view cart containing active item.
* **Expected Result:** Quantity box shows 1 and cart badge shows 1.
* **Actual Result:** Quantity box showed 1 and cart badge header showed 1.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-014-verify-cart-count-pass.png`

---

### TC-015: Continue Shopping from Cart
* **Test Case ID:** `TC-015`
* **Test Title:** Continue shopping from cart
* **Module:** Cart
* **Objective:** Verify navigation back to product catalogue from cart.
* **Preconditions:** User is viewing cart with active items.
* **Test Data:** N/A
* **Execution Steps:**
  1. Tap the "Continue Shopping" button.
* **Expected Result:** User is navigated back to Products inventory page.
* **Actual Result:** User was successfully navigated back to Products inventory page.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-015-continue-shopping-pass.png`

---

## Module 4: Checkout

### TC-016: Checkout with Valid Customer Information
* **Test Case ID:** `TC-016`
* **Test Title:** Checkout with valid customer information
* **Module:** Checkout
* **Objective:** Verify successful submission of valid customer details.
* **Preconditions:** User has items in cart and is on checkout info form.
* **Test Data:** `First Name: John` | `Last Name: Doe` | `Postal Code: 10001`
* **Execution Steps:**
  1. Enter valid data into First Name, Last Name, and Zip/Postal Code fields.
  2. Tap the Continue button.
* **Expected Result:** User is navigated to Checkout: Overview page.
* **Actual Result:** User was successfully navigated to Checkout: Overview page.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-016-checkout-valid-info-pass.png`

---

### TC-017: Checkout with Blank First Name
* **Test Case ID:** `TC-017`
* **Test Title:** Checkout with blank first name
* **Module:** Checkout
* **Objective:** Verify system prevents checkout when First Name is blank.
* **Preconditions:** User is on Checkout: Your Information form page.
* **Test Data:** `First Name: [Blank]` | `Last Name: Doe` | `Postal Code: 9300`
* **Execution Steps:**
  1. Leave First Name empty.
  2. Enter Last Name and Postal Code.
  3. Tap Continue.
* **Expected Result:** Progression is blocked and error message appears.
* **Actual Result:** Progression was blocked and error message displayed.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-017-blank-firstname-pass.png`

---

### TC-018: Checkout with Blank Last Name
* **Test Case ID:** `TC-018`
* **Test Title:** Checkout with blank last name
* **Module:** Checkout
* **Objective:** Verify system prevents checkout when Last Name is blank.
* **Preconditions:** User is on Checkout: Your Information form page.
* **Test Data:** `First Name: John` | `Last Name: [Blank]` | `Postal Code: 9302`
* **Execution Steps:**
  1. Enter First Name.
  2. Leave Last Name empty.
  3. Enter Postal Code.
  4. Tap Continue.
* **Expected Result:** Progression is blocked and error message appears.
* **Actual Result:** Progression was blocked and error message displayed.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-018-blank-lastname-pass.png`

---

### TC-019: Checkout with Blank Postal Code
* **Test Case ID:** `TC-019`
* **Test Title:** Checkout with blank postal code
* **Module:** Checkout
* **Objective:** Verify system prevents checkout when Postal Code is blank.
* **Preconditions:** User is on Checkout: Your Information form page.
* **Test Data:** `First Name: John` | `Last Name: Lennon` | `Postal Code: [Blank]`
* **Execution Steps:**
  1. Enter names.
  2. Leave Postal Code empty.
  3. Tap Continue.
* **Expected Result:** Progression is blocked and error message appears.
* **Actual Result:** Progression was blocked and error message displayed.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-019-blank-postalcode-pass.png`

---

### TC-020: Complete Order Successfully
* **Test Case ID:** `TC-020`
* **Test Title:** Complete order successfully
* **Module:** Checkout
* **Objective:** Verify that a user can successfully submit an order from the overview page and reach the order confirmation screen.
* **Preconditions:** User is on the Checkout: Overview page with valid items and customer info entered.
* **Test Data:** N/A
* **Execution Steps:**
  1. Scroll down to the bottom of the Checkout: Overview page.
  2. Tap the "Finish" button.
* **Expected Result:** Order is processed successfully and the user is navigated to the Checkout: Complete! success screen.
* **Actual Result:** Order was processed successfully and the success screen ("Thank you for your order!") was displayed.
* **Status:** `PASS`
* **Evidence Reference:** `screenshots/test-evidence/tc-020-complete-order-pass.png`

---

## Module 5: Bug Verification

### TC-021: Incorrect Product Images (problem_user)
* **Test Case ID:** `TC-021`
* **Test Title:** Incorrect product images (problem_user)
* **Module:** Bug Verification / Product Catalogue
* **Objective:** Verify product images display correctly for problem_user.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: problem_user` | `Password: secret_sauce`
* **Execution Steps:**
  1. Enter credentials (`problem_user` / `secret_sauce`).
  2. Tap Login.
  3. Inspect product images rendered across items on the inventory page.
* **Expected Result:** Each product shows its correct corresponding image.
* **Actual Result:** Incorrect images displayed (e.g. dog image displayed for Sauce Labs Backpack).
* **Status:** `FAIL`
* **Severity / Priority:** Medium / High
* **Linked Defect ID:** `BUG-UI-001`
* **Evidence Reference:** `screenshots/test-evidence/tc-021-broken-images-fail.png`

---

### TC-022: Sorting Broken (error_user)
* **Test Case ID:** `TC-022`
* **Test Title:** Sorting broken (error_user)
* **Module:** Bug Verification / Product Catalogue
* **Objective:** Verify product sorting works correctly for error_user.
* **Preconditions:** User is on the login page.
* **Test Data:** `Username: error_user` | `Password: secret_sauce`
* **Execution Steps:**
  1. Enter credentials (`error_user` / `secret_sauce`).
  2. Tap Login.
  3. Open sort dropdown menu.
  4. Select any sort option.
* **Expected Result:** Products re-order according to selected sort criteria with no errors.
* **Actual Result:** Error popup displayed: "Sorting is broken! This error has been reported to Backtrace." Sorting does not apply.
* **Status:** `FAIL`
* **Severity / Priority:** High / High
* **Linked Defect ID:** `BUG-FUNC-002`
* **Evidence Reference:** `screenshots/test-evidence/tc-022-sort-broken-fail.png`
