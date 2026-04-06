# 🤖 testRigor AI-Driven Regression Suite: Swag Labs

This document contains the **Natural Language Processing (NLP)** automation logic for a 25-case regression suite. These tests leverage Generative AI to identify elements by human-readable labels rather than fragile XPaths.

 Test Categories
1. End-to-End (E2E) Purchase Flows
2. Cart Management & Logic
3. Session Persistence (Login/Logout/Reload)
4. UI & Sorting Validations

---

Automation Logic (NLP Scripts)

1. Full E2E Purchase Flow (Multiple Items + Tax Validation)
```text
login
click "Add to cart" below the "Sauce Labs Backpack"
click "Add to cart button for Sauce Labs Bike Light" using ai
click "Shopping cart icon" using ai
click "Checkout"
enter "John" into "First Name"
enter "Doe" into "Last Name"
enter "12345" into "Zip/Postal Code"
click "Continue button" using ai
scroll down
check that page contains "Item total: $39.98"
check that page contains "Tax: $3.20"
login
click "Add to cart" below the "Sauce Labs Backpack"
click "Add to cart" below the "Sauce Labs Bike Light"
check that page contains "2"
click "Sauce Labs Backpack"
check that page contains "2"
click "Back to products"
reload
check that page contains "2"
click "Open Menu"
click "Logout"
login
check that page contains "2"
click "Shopping cart icon at top right" using ai
login
click "Add to cart" below the "Sauce Labs Backpack"
click "Add to cart button next to Sauce Labs Bike Light" using ai
scroll down
click "Add to cart button next to Sauce Labs Fleece Jacket" using ai
scroll up
click "Shopping cart icon with badge showing 4" using ai
click "Remove" below the "Sauce Labs Bike Light"
check that page contains "3"
check that page does not contain "Sauce Labs Bike Light"
login
select "Price (low to high)" from "Name (A to Z)"
check that page contains "Price (low to high)"
check that page contains "$7.99"
check that page contains "$9.99"
check that page contains "$15.99"
check that page contains "$29.99"
check that page contains "$49.99"
login
click "hamburger menu icon" using ai
click "Logout"
check that page contains "Login"
check that page contains "Username"
check that page contains "Password"
check that page contains "Total: $43.18"
click "Finish button" using ai
check that page contains "Checkout: Complete!"
check that page contains "Thank you for your order!"
