"# Automation_Test_Store_website" 
# 🧪 Automation Test Store Website – Automated Testing Framework

This repository contains the automated test scripts and framework used to test the [AutomationTestStore](https://automationteststore.com) demo e-commerce website.  
It is part of a larger QA project developed for the ICT Upskilling Program at Al Hussein Technical University (HTU).

---

## 🔧 Technologies Used

- **Language**: Java
- **Automation Tool**: Selenium WebDriver
- **Test Framework**: TestNG
- **IDE**: Eclipse
- **Browser**: Chrome (via ChromeDriver)
- **Test Report**: TestNG Reports

---

## 🗂 Project Structure

FinalProject/<br>
├── src/<br>
│ ├── main/java/FinalProject/<br>
│ │ ├── AppTest.java # Contains automation test cases<br>
│ │ └── TestData.java # Test data & browser setup<br>
├── testng.xml # TestNG suite configuration<br>
├── screenshots/ # Screenshots of test execution (optional)<br>
├── test-reports/ # TestNG HTML reports<br>
└── README.md # Project overview<br>

# 📂 FinalProject – Selenium Test Classes

This folder contains the core Java classes used for automated testing of the [AutomationTestStore](https://automationteststore.com) website using **Selenium WebDriver** and **TestNG**.

---

## 📁 Files Overview

### 🔹 `AppTest.java`

- This class contains all **automation test cases**.
- It covers key functionalities such as:
  - Home page accessibility
  - User registration
  - Login and logout
  - Product search and filtering
  - Add to cart and checkout process
  - Contact form submission
- Test cases are annotated with `@Test` and organized using **TestNG**.

  
## 📄 Description

This project is a Selenium TestNG automation suite developed to test core functionalities of the [AutomationTestStore](https://automationteststore.com) website. It simulates a complete user journey from homepage access to checkout and contact form submission.

The main test file is `AppTest.java`, which contains 10 functional test cases. It also integrates screenshot capturing and optional database logging of user registration data.

---

## 🚦 Test Scenarios in `AppTest.java`

| Test # | Method Name                | Description |
|--------|----------------------------|-------------|
| 1️⃣    | `HomepageAccessibility`    | Checks if the homepage loads and captures a screenshot |
| 2️⃣    | `UserRegistrationProcess`  | Automates the full user registration form and inserts data into a database |
| 3️⃣    | `UserLoginFunctionality`   | Logs in using the previously registered user |
| 4️⃣    | `ProductSearchFunctionality` | Searches for the word "Shampoo" and verifies product results |
| 5️⃣    | `FilteringSearchResults`   | Filters the search results by "Price Low > High" and verifies sorting |
| 6️⃣    | `ViewingProductDetails`    | Clicks a random product from "Latest Products" and checks its detail view |
| 7️⃣    | `AddingProductsToCart`     | Adds the product to the cart and confirms it appears there |
| 8️⃣    | `ViewingAndModifyingShoppingCart` | Changes product quantity in the cart and verifies the total price |
| 9️⃣    | `ProceedingToCheckout`     | Completes checkout and verifies success message |
| 🔟    | `ContactFormSubmission`     | Submits the "Contact Us" form and checks the confirmation message |

---


### 🔹 `TestData.java`

- This class handles:
  - **WebDriver setup and configuration**
  - **Dynamic test data generation** (e.g., random emails and usernames)
  - Common **expected results**
  - Utility methods used by the test scripts
- It is used by `AppTest.java` through class extension or shared access.

---


## 🚀 How It Works

1. `TestData.java` sets up the browser and test data.
2. `AppTest.java` imports this setup and runs end-to-end test cases.
3. Execution is managed using `testng.xml` (located in the main test folder).
4. Results are shown in the TestNG HTML reports.

---

## ✅ Best Practices Followed

- **Page Object Model (POM)**: Modular structure and reusable methods
- **Data-driven testing**: Random input generation to avoid test conflicts
- **Structured test cases**: Each test has clear setup, action, and assertion

---
