# 💳 DFS (Dmoney Financial Service) — Manual Testing Project

A complete manual testing documentation project for a **Dmoney Financial Service (DFS)** system — similar to bKash/Nagad — covering user registration, authentication, and customer transactions.

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
   git clone https://github.com/Ummejami/Dmoney-Manual-Testing.git
   cd Dmoney-Manual-Testing
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


---

## 🔐 System Roles & Test Users

| Role | Email | Phone | Status |
|------|-------|-------|--------|
| Admin | admin@dmoney.com | 01XXXXXXXXX | Active (seeded) |
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


---

## 📊 Test Execution Summary

| Module | Total TCs | Passed | Failed | Blocked |
|--------|-----------|--------|--------|---------|
| Send Money | 12 | 10 | 2 | 0 |
| Bank Cash-In (Stripe) | 10 | 8 | 2 | 0 |
| Payment to Merchant | 10 | 10 | 0 | 0 |
| Cash Out | 14 | 14 | 0 | 0 |

---

## 📚 Concepts Covered

- ✅ Acceptance Testing vs Acceptance Criteria
- ✅ Decision Table Testing vs Decision Coverage
- ✅ Exit Criteria vs Test Completion Report

---

## 📸 Jira Work Screenshots

### 🗂️ Backlog
![Backlog](JJira%20Image/Backlog.png)

### ⚡ Active Sprint
![ActiveSprint](JJira%20Image/ActiveSprint.png)

### 📊 Burn Down
![BurnDown](JJira%20Image/BurnDown.png)

### 📈 Burn Down Summary
![BurnDownSummary](JJira%20Image/BurnDownSummay.png)

### 🎯 Priority
![Priority](JJira%20Image/Priority.png)

### 🧩 Subtask
![Subtask](JJira%20Image/Subtask.png)

### 📄 Summary
![Summary](JJira%20Image/Summary.png)

### 👥 Team Workload
![TeamWorkload](JJira%20Image/TeamWorkload.png)

### 📝 Type of Works
![TypeOfWorks](JJira%20Image/TypeOfWorks.png)

## 📄 License

This project is for educational/assessment purposes only.
