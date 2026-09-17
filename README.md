
# VRIP — Vendor Reliability Intelligence Platform

## Project Overview

**Vendor Reliability Intelligence Platform (VRIP)** is a full-stack web application designed to help organizations manage vendors, procurement activities, purchase orders, vendor performance, reliability scores, risk levels, contracts, notifications, reports, and supply-chain analytics through a centralized platform.

The system provides data-driven insights into vendor reliability and procurement operations, helping organizations monitor supplier performance and identify potential operational risks.

---

## Key Features

* User Registration and Login
* JWT-based Authentication
* Role-Based Access Control (RBAC)
* Vendor Registration and Management
* Vendor Reliability Scoring
* Vendor Risk-Level Classification
* Procurement Request Management
* Purchase Order Management
* Vendor Performance Monitoring
* Contract and Compliance Monitoring
* Notifications and Alerts
* Audit Log Management
* Reports and Analytics
* Supply Chain Analytics Dashboard
* Excel Report Export
* Dashboard with Key Procurement and Vendor Metrics

---

## Technology Stack

### Frontend

* Angular
* TypeScript
* HTML5
* CSS3
* Chart.js

### Backend

* Python
* FastAPI
* SQLAlchemy
* REST APIs
* JWT Authentication

### Database

* PostgreSQL

### Development Tools

* Visual Studio Code
* Git
* GitHub

---

## Vendor Reliability Scoring

The platform calculates vendor reliability using four performance factors:

* Delivery Score
* Quality Score
* Payment Score
* Compliance Score

The overall reliability score is calculated based on the average of these factors.

### Risk Classification

| Reliability Score | Risk Level |
| ----------------- | ---------- |
| 80 – 100          | Low        |
| 50 – 79.99        | Medium     |
| Below 50          | High       |

---

## System Modules

### 1. Authentication and Authorization

Provides secure user registration, login, JWT-based authentication, and role-based access control.

### 2. Vendor Management

Allows users to register, view, update, and monitor vendor information and reliability performance.

### 3. Procurement Management

Manages procurement requests, budgets, quantities, vendors, and procurement status.

### 4. Purchase Order Management

Provides management of purchase orders, order details, delivery information, amounts, and order status.

### 5. Vendor Performance

Tracks vendor performance indicators and calculates reliability scores and risk levels.

### 6. Contracts and Compliance

Supports contract monitoring and vendor compliance tracking.

### 7. Notifications and Alerts

Displays system activities, risk warnings, critical alerts, and operational updates.

### 8. Reports and Analytics

Provides reports and analytical information for vendor and procurement performance.

### 9. Supply Chain Analytics

Provides insights into supplier orders, order status, product categories, compliance, and defective units.

### 10. Audit Logs

Maintains records of important system activities and user actions.

---

## Project Structure

```text
VRIP-Vendor-Reliability-Intelligence-Platform/
│
├── backend/
│   ├── app/
│   │   ├── models/
│   │   ├── routers/
│   │   ├── schemas/
│   │   ├── services/
│   │   ├── database.py
│   │   └── main.py
│   │
│   ├── data/
│   ├── requirements.txt
│   └── README.md
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   ├── assets/
│   │   └── ...
│   ├── package.json
│   └── angular.json
│
├── .gitignore
└── README.md
```

---

## Installation and Setup

### Prerequisites

Make sure the following are installed:

* Python 3.12+
* Node.js
* Angular CLI
* PostgreSQL
* Git

---

## Backend Setup

Open a terminal in the project root and run:

```bash
cd backend
```

Create and activate a virtual environment:

```bash
python -m venv venv
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Start the FastAPI server:

```bash
python -m uvicorn app.main:app --reload
```

The backend will be available at:

```text
http://127.0.0.1:8000
```

API documentation:

```text
http://127.0.0.1:8000/docs
```

---

## Frontend Setup

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the Angular development server:

```bash
ng serve
```

The frontend will be available at:

```text
http://localhost:4200
```

---

## Application Workflow

```text
User Login
    ↓
Dashboard
    ↓
Vendor Management
    ↓
Vendor Reliability Evaluation
    ↓
Risk Classification
    ↓
Procurement Management
    ↓
Purchase Order Management
    ↓
Performance & Compliance Monitoring
    ↓
Reports & Analytics
    ↓
Supply Chain Insights
```

---

## Project Objectives

* Centralize vendor and procurement information.
* Monitor vendor reliability and performance.
* Identify vendor risk levels using performance scores.
* Improve procurement visibility.
* Track purchase orders and supplier activities.
* Monitor compliance and operational performance.
* Provide analytical insights through dashboards and reports.
* Support data-driven procurement management.

---

## Future Enhancements

* Cloud deployment
* Advanced predictive risk analytics
* Automated email notifications
* AI-based vendor risk prediction
* Advanced procurement forecasting
* Integration with external ERP systems
* Mobile-responsive enhancements
* Automated report scheduling

---

## Project Repository

**GitHub:**
https://github.com/Hrishi18162/VRIP-Vendor-Reliability-Intelligence-Platform

---

## Author

**Hrishitha Kotte**

Vendor Reliability Intelligence Platform
Full Stack Development Project
