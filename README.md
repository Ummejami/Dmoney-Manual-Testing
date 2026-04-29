# 💳 MFS (Mobile Financial Service) — Manual Testing Project

A complete manual testing documentation project for a **Mobile Financial Service (MFS)** system — similar to bKash/Nagad — covering user registration, authentication, and customer transactions.

---

## 📋 Project Overview

This project contains end-to-end manual testing artifacts for an MFS platform built with a role-based financial system. The platform supports five roles: **Admin, Agent, Customer, Merchant, and SYSTEM**, with controlled money flow and transaction limits.

---

## 🛠️ Environment Setup

### Prerequisites

| Tool | Purpose |
|------|---------|
| VS Code | Local development & file management |
| DBeaver | Database connection & query execution |
| Postman / Browser | API / UI testing |
| Git | Version control |

### Local Setup Steps

1. **Clone the repository**
```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
```

2. **Open in VS Code**
```bash
   code .
```

3. **Database Connection via DBeaver**
   - Open DBeaver → New Database Connection
   - Select your DB type (MySQL / PostgreSQL)
   - Enter host, port, database name, username & password
   - Test connection → Finish

---

## 📁 Project Structure
📦 mfs-manual-testing
 ┣ 📂 test-plan
 ┃ ┗ 📄 test-estimation.md
 ┣ 📂 acceptance-criteria
 ┃ ┗ 📄 acceptance-criteria.md
 ┣ 📂 test-cases
 ┃ ┗ 📄 customer-transaction-test-cases.xlsx
 ┣ 📂 test-execution
 ┃ ┗ 📄 execution-report.xlsx
 ┣ 📂 bug-report
 ┃ ┗ 📄 exploratory-testing-bugs.xlsx
 ┣ 📂 checklist
 ┃ ┗ 📄 full-system-checklist.xlsx
 ┗ 📄 README.md
---

## ✅ Tasks Completed

| # | Task | Status |
|---|------|--------|
| 1 | Test Estimation — Customer Transaction Module | ✅ Done |
| 2 | Acceptance Criteria — Registration, Auth & Customer Transactions | ✅ Done |
| 3 | Test Data — Created Customer, Agent, Merchant & Admin activation | ✅ Done |
| 4 | Test Cases (Positive & Negative) — Customer Transactions | ✅ Done |
| 5 | Test Execution Report with Actual Results & Status | ✅ Done |
| 6 | Exploratory Testing — Full System Bug Report | ✅ Done |
| 7 | Full System Checklist | ✅ Done |
| 8 | Acceptance Testing vs Acceptance Criteria (Difference) | ✅ Done |
| 9 | Decision Table Testing vs Decision Coverage (Difference) | ✅ Done |
| 10 | Exit Criteria vs Test Completion Report (Difference) | ✅ Done |

---

## 🔐 System Roles & Test Users

| Role | Email | Phone | Status |
|------|-------|-------|--------|
| Admin | admin@test.com | 01XXXXXXXXX | Active (seeded) |
| Agent | agent@test.com | 01XXXXXXXXX | Activated by Admin |
| Customer | customer@test.com | 01XXXXXXXXX | Activated by Admin |
| Merchant | merchant@test.com | 01XXXXXXXXX | Activated by Admin |

> ⚠️ All non-admin accounts require Admin approval before transactions are enabled.

---

## 💰 Module Coverage

### Customer Transactions
- **Cash-Out** via Agent (1% fee, min 5 BDT → SYSTEM; 2.5% commission → Agent)
- **Send Money** P2P (flat 5 BDT fee → SYSTEM)
- **Bank Cash-In** via Stripe (10–10,000 BDT, wallet cap 10,000 BDT)
- **Payment to Merchant** (1% fee, min 5 BDT → Merchant)

### Transaction Limits (Customer)
| Limit Type | Value |
|-----------|-------|
| Max per day (BDT) | 5,000 |
| Max per month (BDT) | 50,000 |
| Max transactions/day | 10 |
| Max transactions/month | 50 |

---

## 🐛 Bug Report

Exploratory testing was performed on the full system. Bug reports are documented with:
- Bug ID
- Module
- Summary
- Steps to Reproduce
- Expected vs Actual Result
- Severity & Priority
- Status

📄 See: [`bug-report/exploratory-testing-bugs.xlsx`](./bug-report/exploratory-testing-bugs.xlsx)

---

## 📊 Test Execution Summary

| Module | Total TCs | Passed | Failed | Blocked |
|--------|-----------|--------|--------|---------|
| Send Money | — | — | — | — |
| Bank Cash-In (Stripe) | — | — | — | — |
| Payment to Merchant | — | — | — | — |

> 📝 Fill in the numbers after execution is complete.

---

## 📚 Concepts Covered

- ✅ Acceptance Testing vs Acceptance Criteria
- ✅ Decision Table Testing vs Decision Coverage
- ✅ Exit Criteria vs Test Completion Report

---

## 👤 Author

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [your-linkedin](https://linkedin.com/in/your-profile)

---

## 📄 License

This project is for educational/assessment purposes only.
