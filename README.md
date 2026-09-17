
# VRIP — Vendor Reliability Intelligence Platform

## Project Overview

The **Vendor Reliability Intelligence Platform (VRIP)** is a full-stack web application designed to help organizations manage vendors, procurement activities, purchase orders, vendor performance, compliance, and supply-chain operations.

The platform provides data-driven insights into vendor reliability and procurement risk through reliability scoring, analytics, reports, notifications, and audit tracking.

---

## Objectives

* Manage vendor information in a centralized system.
* Monitor vendor performance and reliability.
* Manage procurement requests and purchase orders.
* Calculate vendor reliability and risk levels.
* Monitor contracts and compliance.
* Provide dashboards and analytics for decision-making.
* Generate reports and export business data.
* Track system activities through notifications and audit logs.
* Analyze supply-chain and procurement data.

---

## Key Features

### Authentication and Authorization

* User registration and login.
* JWT-based authentication.
* Role-based access control.
* Protected application routes.
* Secure API authorization.

### Vendor Management

* Vendor registration.
* Vendor information management.
* Vendor performance monitoring.
* Vendor reliability score calculation.
* Vendor risk-level classification.
* Vendor status management.

### Procurement Management

* Create and manage procurement requests.
* Track procurement status.
* Associate procurement requests with vendors.
* Monitor procurement budgets and quantities.

### Purchase Order Management

* Create and manage purchase orders.
* Assign purchase orders to vendors.
* Track order status.
* Monitor order amounts and delivery information.
* Manage defective units and compliance information.

### Vendor Performance and Risk

Vendor reliability is calculated using four performance factors:

* Delivery Score
* Quality Score
* Payment Score
* Compliance Score

The platform calculates an overall reliability score and classifies vendors into risk levels.

### Contracts and Compliance

* Contract management.
* Compliance monitoring.
* Vendor compliance tracking.
* Contract-related information management.

### Notifications and Audit Logs

* System notifications.
* Risk warnings.
* Activity monitoring.
* Audit log tracking.
* Important operational alerts.

### Reports and Analytics

* Vendor reports.
* Procurement reports.
* Performance analytics.
* Dashboard statistics.
* Data export functionality.
* Supply-chain analytics.

### Supply Chain Analytics

The platform provides supply-chain insights including:

* Order status analysis.
* Supplier performance.
* Product/category analysis.
* Compliance analysis.
* Defective-unit analysis.
* Procurement value analysis.

---

## Technology Stack

### Frontend

* Angular
* TypeScript
* HTML5
* CSS3
* Chart.js
* Angular Router
* Angular HTTP Client
* Route Guards
* HTTP Interceptors

### Backend

* Python
* FastAPI
* SQLAlchemy
* REST APIs
* JWT Authentication
* Role-Based Access Control
* ReportLab
* OpenPyXL

### Database

* PostgreSQL

### Development Tools

* Visual Studio Code
* Git
* GitHub
* Swagger / OpenAPI

---

## Vendor Reliability Scoring

The platform evaluates vendor reliability using four performance parameters:

| Parameter        | Description                           |
| ---------------- | ------------------------------------- |
| Delivery Score   | Measures delivery performance         |
| Quality Score    | Measures product/service quality      |
| Payment Score    | Measures payment-related performance  |
| Compliance Score | Measures compliance with requirements |

The overall reliability score is calculated using the average of these four scores.

### Risk Classification

| Reliability Score | Risk Level |
| ----------------- | ---------- |
| 80–100            | Low        |
| 50–79.99          | Medium     |
| Below 50          | High       |

This classification helps organizations identify vendors that may require additional monitoring.

---

## System Architecture

```text
                    VRIP PLATFORM

                         |
          +--------------+--------------+
          |                             |
      Angular                        FastAPI
      Frontend                       Backend
          |                             |
          |                         REST APIs
          |                             |
          +--------------+--------------+
                         |
                    PostgreSQL
                     Database
                         |
          +--------------+--------------+
          |              |               |
       Vendors       Procurement    Analytics
          |              |               |
       Purchase       Reports        Risk Analysis
       Orders        Notifications   Supply Chain
```

---

## Project Structure

```text
VRIP-Vendor-Reliability-Intelligence-Platform/
│
├── backend/
│   ├── app/
│   │   ├── routers/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── services/
│   │   └── main.py
│   │
│   ├── data/
│   ├── requirements.txt
│   └── ...
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

Install the following software before running the project:

* Python 3.12 or later
* Node.js
* Angular CLI
* PostgreSQL
* Git
* Visual Studio Code

---

## Backend Setup

Open a terminal and navigate to the backend directory:

```bash
cd backend
```

Create and activate a Python virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```powershell
venv\Scripts\activate
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Configure the database connection and required environment variables.

Start the FastAPI backend:

```bash
python -m uvicorn app.main:app --reload
```

The backend will run at:

```text
http://127.0.0.1:8000
```

### API Documentation

FastAPI Swagger documentation is available at:

```text
http://127.0.0.1:8000/docs
```

---

## Frontend Setup

Open another terminal and navigate to the frontend directory:

```bash
cd frontend
```

Install the required Node.js packages:

```bash
npm install
```

Start the Angular development server:

```bash
ng serve
```

The frontend will run at:

```text
http://localhost:4200
```

---

## Application Workflow

```text
User
  |
  v
Login / Registration
  |
  v
Dashboard
  |
  +------------------+
  |                  |
  v                  v
Vendors          Procurement
  |                  |
  v                  v
Vendor Risk      Purchase Orders
  |                  |
  +--------+---------+
           |
           v
     Analytics & Reports
           |
           v
 Notifications & Audit Logs
           |
           v
     Supply Chain Insights
```

---

## Security

The platform implements security features including:

* JWT-based authentication.
* Password-based user authentication.
* Role-based authorization.
* Protected Angular routes.
* HTTP authorization interceptors.
* Backend API authorization.
* Restricted access to sensitive operations.

---

## Reporting and Analytics

VRIP provides reporting and analytical capabilities for monitoring business operations.

Reports and dashboards can provide information related to:

* Vendor reliability.
* Vendor risk levels.
* Procurement activities.
* Purchase orders.
* Vendor performance.
* Compliance.
* Supply-chain operations.
* System activities.

Reports can also be exported for further analysis.

---

## Future Enhancements

Possible future improvements include:

* Advanced predictive vendor-risk analysis.
* Machine-learning-based vendor reliability prediction.
* Automated email notifications.
* Advanced supplier performance benchmarking.
* Cloud deployment.
* Docker containerization.
* Enhanced data visualization.
* Automated scheduled reports.
* Advanced procurement forecasting.

---

## Repository

**GitHub Repository:**

https://github.com/Hrishi18162/VRIP-Vendor-Reliability-Intelligence-Platform

---

## Author

**Hrishitha Kotte**

Vendor Reliability Intelligence Platform — Full Stack Development Project
