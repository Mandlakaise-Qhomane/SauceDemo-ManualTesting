# Bug Report: Sorting Mechanism Triggers Backtrace Error Exception

**Bug ID:** BUG-FUNC-002  
**Severity:** High  
**Priority:** High  
**Target Module:** Product Catalogue / Sorting  
**Environment:** Sauce Demo Production Web Client  
**Test Case Reference:** `TC-022`[span_9](start_span)[span_9](end_span)  

---

## Executive Summary
When authenticating as `error_user`, attempting to change the product sorting criteria triggers an error modal dialogue ("Sorting is broken! This error has been reported to Backtrace.") and fails to re-order the inventory list[span_10](start_span)[span_10](end_span).

---

## Steps to Reproduce
1. Navigate to `https://www.saucedemo.com/`[span_11](start_span)[span_11](end_span).
2. Login using credentials: `error_user` / `secret_sauce`[span_12](start_span)[span_12](end_span).
3. Click on the product sorting dropdown menu[span_13](start_span)[span_13](end_span).
4. Select any sort filter (e.g., Price low-to-high, Name Z-to-A)[span_14](start_span)[span_14](end_span).

---

## Expected Result
The catalog re-orders correctly according to the selected criteria without runtime error popups[span_15](start_span)[span_15](end_span).

---

## Actual Result
An error popup is displayed: `"Sorting is broken! This error has been reported to Backtrace."` and catalog ordering remains unchanged[span_16](start_span)[span_16](end_span).

---

## Evidence Reference
`screenshots/test-evidence/tc-022-sort-broken-fail.png`[span_17](start_span)[span_17](end_span)
