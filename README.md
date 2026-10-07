# 💳 PhonePe Wallet — Full-Stack Digital Wallet

A modern **digital wallet application inspired by PhonePe**, built with **React.js** and **Spring Boot**. The application provides a seamless interface for user authentication, wallet management, peer-to-peer money transfers, and transaction tracking through a modular full-stack architecture.

> **React + Spring Boot + REST APIs**

---

## ✨ Overview

PhonePe Wallet is a full-stack digital payment application designed to simulate core wallet operations in a real-world payment platform.

The project focuses on building a clean frontend architecture, integrating RESTful APIs, managing application state, and implementing reusable components for wallet and transaction workflows.

### Core Workflow

```text
Register / Login
      ↓
   Dashboard
      ↓
Wallet Balance
   ↙       ↘
Add Money   Send Money
               ↓
          Transaction
               ↓
      Transaction History
```

---

## 🚀 Key Features

### 🔐 Authentication
- User registration and login
- Client-side form validation
- Authentication-aware application flow
- Dedicated authentication components

### 💰 Wallet Management
- Real-time wallet balance display
- Add money functionality
- Wallet balance updates
- Quick-access wallet actions

### 💸 Money Transfers
- Peer-to-peer money transfer
- Transfer amount validation
- Transaction confirmation
- Automatic wallet balance updates

### 📊 Transaction Management
- Transaction history
- Individual transaction details
- Sender and receiver information
- Transaction amount and status

### 🎨 User Experience
- Responsive interface
- Reusable React components
- Modal-based workflows
- Toast notifications
- Loading indicators
- Error handling and user feedback

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **React.js** | Frontend UI development |
| **Vite** | Frontend build tooling |
| **JavaScript (ES6+)** | Application logic |
| **Spring Boot** | Backend & REST APIs |
| **Axios** | Client-server communication |
| **CSS3** | Styling & responsive UI |
| **Java** | Backend development |
| **Git & GitHub** | Version control |

---

## 🏗️ System Architecture

```text
                    ┌──────────────────────┐
                    │      React.js        │
                    │      Frontend        │
                    └──────────┬───────────┘
                               │
                          REST APIs
                               │
                               ▼
                    ┌──────────────────────┐
                    │     Spring Boot      │
                    │       Backend        │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              ▼                ▼                ▼
        Authentication    Wallet Services   Transactions
```

The frontend follows a **component-based architecture**, while backend functionality is exposed through RESTful APIs.

---

## 📂 Project Structure

```text
src/
│
├── api/
│   └── index.js
│
├── components/
│   ├── auth/
│   │   ├── LoginForm.jsx
│   │   └── RegisterForm.jsx
│   │
│   ├── layout/
│   │   └── Header.jsx
│   │
│   ├── transaction/
│   │   ├── SendMoneyModal.jsx
│   │   ├── TransactionList.jsx
│   │   └── TransactionRow.jsx
│   │
│   ├── ui/
│   │   ├── Button.jsx
│   │   ├── Icon.jsx
│   │   ├── Input.jsx
│   │   ├── Modal.jsx
│   │   ├── Spinner.jsx
│   │   └── Toast.jsx
│   │
│   └── wallet/
│       ├── AddMoneyModal.jsx
│       ├── BalanceCard.jsx
│       └── QuickActions.jsx
│
├── hooks/
│   ├── useToast.js
│   └── useWallet.js
│
├── pages/
│   ├── AuthPage.jsx
│   └── DashboardPage.jsx
│
├── styles/
│   └── global.css
│
├── utils.js
├── App.jsx
└── main.jsx
```

---

## ⚙️ Getting Started

### Prerequisites

- **Node.js 18+**
- **npm**
- **Java 17+**
- Spring Boot backend

### Clone the Repository

```bash
git clone https://github.com/harshakoushika/PhonePe_Frontend.git

cd PhonePe_Frontend
```

### Install Dependencies

```bash
npm install
```

### Start the Backend

Start the Spring Boot backend on:

```text
http://localhost:8080
```

### Start the Frontend

```bash
npm run dev
```

Open the application at:

```text
http://localhost:5173
```

The Vite development server proxies `/api` requests to the Spring Boot backend.

---

## 🔄 Application Flow

```text
┌──────────────────┐
│ User Registration│
│    / Login       │
└────────┬─────────┘
         ↓
┌──────────────────┐
│    Dashboard     │
└────────┬─────────┘
         ↓
┌──────────────────┐
│  Wallet Balance  │
└───────┬──────────┘
        │
   ┌────┴─────┐
   ↓          ↓
Add Money   Send Money
   │          │
   │          ↓
   │     Transaction
   │          │
   └────┬─────┘
        ↓
┌──────────────────┐
│ Transaction List │
└──────────────────┘
```

---

## 🧩 Component Architecture

The frontend is organized into reusable feature-based modules:

**Authentication**
- `LoginForm`
- `RegisterForm`

**Wallet
