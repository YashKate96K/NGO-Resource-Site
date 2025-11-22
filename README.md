# NGO Dashboard: Trust, Transparency, Teamwork

A modern, offline-capable, role-based dashboard for NGOs, built with React.js (frontend), Flask (backend), and a local custom Windsurf CSS framework. Features Admin, Volunteer, and Beneficiary dashboards, accessibility-first design, and full offline support.

## Structure
- `frontend/` — React app, Windsurf CSS, local assets
- `backend/` — Flask API, role-based endpoints
- `shared/` — Fonts, icons, images (all local)

## Features
- Modern, accessible UI/UX
- Role-based dashboards
- Offline support (Service Worker)
- Charts, cards, status indicators
- Mobile-first, responsive
- Deployable to Google App Engine

---

## Getting Started
See each folder for setup instructions.

---

# Bank Management System

## Overview

The **Bank Management System** is a Java-based desktop application designed to simulate basic banking operations with a graphical user interface (GUI). It allows users to create accounts, log in, and perform various banking transactions such as deposits, withdrawals, balance inquiries, and more.

## Features

- **User Authentication:** Signup and login functionality for new and existing users.
- **Account Management:** Create and manage bank accounts.
- **Transactions:** Deposit, withdraw, and check account balance.
- **Mini Statement:** View recent transactions.
- **PIN Management:** Change or reset account PIN.
- **Fast Cash:** Quick withdrawal options.
- **Date Selection:** Uses the JCalendar library for date picking in forms.

## Technology Stack

- **Language:** Java (Desktop Application)
- **GUI:** Java Swing
- **External Library:** [JCalendar](https://toedter.com/jcalendar/) (`com.toedter.calendar.JDateChooser`)

## Project Structure

```
bank managment system/
├── bank/
│   └── management/
│       └── system/
│           ├── BalanceEnquriy.java
│           ├── Con1.java
│           ├── Deposit.java
│           ├── Fastcash.java
│           ├── JDateChooser.java
│           ├── Mini.java
│           ├── Pin.java
│           ├── Signup.java
│           ├── Signup2.java
│           ├── Signup3.java
│           ├── Withdrawl.java
│           ├── login.java
│           └── main_Class.java
└── lib/
    └── jcalendar-x.x.jar
```

## How to Run

1. **Requirements:**
   - Java JDK (8 or above)
   - JCalendar library (`jcalendar-x.x.jar`)

2. **Compilation:**
   ```sh
   javac -cp ".;lib\\jcalendar-x.x.jar" bank\\management\\system\\*.java
   ```

3. **Manifest File:**  
   Create a file named `manifest.txt` with:
   ```
   Main-Class: bank.management.system.main_Class
   ```

4. **Packaging:**
   ```sh
   jar cfm BankManagementSystem.jar manifest.txt bank\\management\\system\\*.class
   ```

5. **Running:**
   ```sh
   java -cp "BankManagementSystem.jar;lib\\jcalendar-x.x.jar" bank.management.system.main_Class
   ```

## Notes

- The application is intended for educational and demonstration purposes.
- Ensure the `lib` directory with the JCalendar JAR is present for the application to function correctly.
- All data is handled in-memory unless additional database integration is implemented.

---
