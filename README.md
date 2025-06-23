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
