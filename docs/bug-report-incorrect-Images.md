# Bug Report: Incorrect Product Images Rendered for Problem User

**Bug ID:** BUG-UI-001  
**Severity:** Medium  
**Priority:** High  
**Target Module:** Product Catalogue  
**Environment:** Sauce Demo Production Web Client  
**Test Case Reference:** `TC-021`[span_0](start_span)[span_0](end_span)  

---

## Executive Summary
When authenticating with the `problem_user` account, the product inventory page renders incorrect image assets across multiple product listings[span_1](start_span)[span_1](end_span). Product placeholders display unrelated images (e.g., a dog photo displayed for the Sauce Labs Backpack)[span_2](start_span)[span_2](end_span).

---

## Steps to Reproduce
1. Navigate to `https://www.saucedemo.com/`[span_3](start_span)[span_3](end_span).
2. Login using credentials: `problem_user` / `secret_sauce`[span_4](start_span)[span_4](end_span).
3. Inspect the product catalog image assets rendered on the inventory screen[span_5](start_span)[span_5](end_span).

---

## Expected Result
Each product listing displays its corresponding product asset image[span_6](start_span)[span_6](end_span).

---

## Actual Result
Incorrect image sources are populated for inventory items (e.g., dog image rendered for Sauce Labs Backpack)[span_7](start_span)[span_7](end_span).

---

## Evidence Reference
`screenshots/test-evidence/tc-021-broken-images-fail.png`[span_8](start_span)[span_8](end_span)
