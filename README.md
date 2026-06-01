# Gmail Compose — Test Case Document

![Status](https://img.shields.io/badge/Status-Not%20Run-lightgrey)
![Version](https://img.shields.io/badge/Version-1.0-blue)
![Priority](https://img.shields.io/badge/Priority-High%20%7C%20Medium-orange)
![Type](https://img.shields.io/badge/Type-Functional%20%7C%20Boundary%20%7C%20Negative-green)

## 📋 Project Overview

| Field | Details |
|-------|---------|
| **Project** | Gmail Web App |
| **Module** | Compose |
| **Version** | 1.0 |
| **Prepared By** | Shanu Shah |
| **Created At** | 2026-05-31 |

This repository contains structured test cases for the **Gmail Compose** feature, covering functional, boundary, and negative test scenarios across key sub-modules.

---

## 📁 Repository Structure

```
gmail-compose-test-cases/
├── README.md
├── Gmail Compose Test Cases    ← Main test case sheet
├── BDD Test Cases              ← Behaviour-Driven Development scenarios
└── Summary                     ← Test execution summary
```

---

## 🧪 Test Coverage

### Sub-Modules Covered

| Sub-Module | Test Cases | Description |
|------------|-----------|-------------|
| **Compose Window** | TC001 – TC003 | Window open, minimize/maximize/close, auto-save draft |
| **Recipient Handling** | TC004 – TC008 | Valid/invalid addresses, autocomplete, multiple recipients, spam limit |
| **Subject Line** | TC009 – TC010 | Empty subject warning, character limit boundary |
| **Body** | TC011 – TC012 | Empty body send, rich text formatting |

---

## 📝 Test Case Summary

| TC ID | Test Case Title | Priority | Type |
|-------|----------------|----------|------|
| TC001 | Verify Compose window opens successfully when user clicks on compose button | High | Functional |
| TC002 | Verify minimise, maximise and close control functions in compose window | High | Functional |
| TC003 | Verify draft email is auto-saved while composing a message | High | Functional |
| TC004 | Verify that system accepts a valid email address in recipient field | High | Functional |
| TC005 | Verify that error message displayed for invalid recipient email address | High | Negative |
| TC006 | Verify auto complete suggestion are displayed for saved contacts | Medium | Functional |
| TC007 | Verify that user can add multiple recipients in the To field | High | Functional |
| TC008 | Verify system display a warning when recipients limit exceeded | Medium | Boundary |
| TC009 | Verify warning message is displayed when sending email without subject | High | Functional |
| TC010 | Verify user enter long subject line exceeding the standard character limit | Medium | Boundary |
| TC011 | Verify email can be sent successfully with an empty message body | Medium | Functional |
| TC012 | Verify rich text formatting options (Bold, Italic, Underline) | Medium | Functional |

---

## ✅ Test Case Structure

Each test case follows this standard format:

```
TC ID          → Unique identifier (e.g., TC001)
Module         → Gmail
Sub-Module     → Compose Window / Recipient Handling / Subject Line / Body
Test Case Title → Description of what is being tested
Pre-conditions → System state required before test execution
Test Steps     → Step-by-step actions to perform
Expected Result → The anticipated outcome
Actual Result  → Filled during test execution
Status         → Not Run / Pass / Fail / Blocked
Priority       → High / Medium / Low
Type           → Functional / Boundary / Negative
```

---

## 🚦 Test Status Legend

| Status | Description |
|--------|-------------|
| 🔘 Not Run | Test has not been executed yet |
| ✅ Pass | Test executed and passed |
| ❌ Fail | Test executed and failed |
| 🚫 Blocked | Test blocked due to dependency or environment issue |

---

## 🔖 Test Types

- **Functional** — Verifies that a feature behaves as expected under normal conditions.
- **Negative** — Verifies that the system handles invalid input or unexpected user behaviour gracefully.
- **Boundary** — Verifies behaviour at the edges of input limits (e.g., max character count, recipient limits).

---

## 🚀 How to Use

1. Open the spreadsheet file (`Gmail Compose Test Cases`).
2. Navigate to the relevant sheet (`Gmail Compose Test Cases`, `BDD Test Cases`, or `Summary`).
3. Execute test cases in the listed order.
4. Fill in the **Actual Result** and update the **Status** column after each test run.
5. Review the **Summary** sheet for overall pass/fail metrics.

---

## 🤝 Contributing

If you identify missing test scenarios or want to improve existing ones:

1. Fork this repository.
2. Create a new branch: `git checkout -b feature/add-new-test-cases`
3. Add or update test cases following the existing format.
4. Submit a Pull Request with a clear description of changes.

---

## 📬 Contact

**Prepared by:** Shanu Shah  
For queries or feedback, please raise an issue in this repository.
