
# VRIP Vendor Reliability Intelligence Platform

## Project Overview

**Vendor Reliability Intelligence Platform (VRIP)** is a full-stack web application designed to help organizations manage vendors, procurement activities, purchase orders, vendor performance, reliability scores, risk levels, contracts, compliance, notifications, reports, and supply-chain analytics through a centralized platform.

The platform provides data-driven insights into vendor reliability and procurement operations, helping organizations monitor supplier performance and identify potential operational risks.

---

## Objectives

* Centralize vendor and procurement information.
* Monitor vendor reliability and performance.
* Calculate vendor reliability scores.
* Classify vendors based on risk levels.
* Manage procurement requests and purchase orders.
* Monitor vendor compliance and performance.
* Provide reports and analytical insights.
* Support supply-chain monitoring and decision-making.

---

## Key Features

### Authentication & Authorization

* User registration and login
* JWT-based authentication
* Role-Based Access Control (RBAC)
* Protected application routes

### Vendor Management

* Vendor registration
* Vendor information management
* Vendor performance monitoring
* Reliability score calculation
* Risk-level classification

### Procurement Management

* Procurement request creation
* Vendor assignment
* Budget and quantity management
* Procurement status tracking

### Purchase Order Management

* Purchase order creation
* Vendor and procurement association
* Order amount and quantity tracking
* Delivery status monitoring
* Purchase order status management

### Vendor Performance & Risk

* Delivery performance
* Quality performance
* Payment performance
* Compliance performance
* Overall reliability score
* Low, Medium, and High risk classification

### Contracts & Compliance

* Contract monitoring
* Vendor compliance tracking
* Compliance status management

### Notifications & Audit Logs

* System notifications
* Risk warnings
* Critical alerts
* Activity monitoring
* Audit log tracking

### Reports & Analytics

* Vendor reports
* Procurement reports
* Performance analytics
* Dashboard statistics
* Excel report export

### Supply Chain Analytics

* Supplier analysis
* Order status analysis
* Product category analysis
* Compliance analysis
* Defective-unit analysis
* Supply-chain dashboard

---

## Technology Stack

### Frontend

The frontend is developed using **Angular** and provides the user interface for managing vendors, procurement, purchase orders, reports, notifications, and analytics.

**Technologies:**

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

The backend is developed using **Python FastAPI** and provides REST APIs, authentication, business logic, database operations, reliability calculations, reports, and analytics.

**Technologies:**

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

VRIP evaluates vendor reliability using four major performance factors:

1. **Delivery Score**
2. **Quality Score**
3. **Payment Score**
4. **Compliance Score**

The overall reliability score is calculated using the average of these performance scores.

### Risk Classification

| Reliability Score | Risk Level |
| ----------------- | ---------- |
| 80 – 100          | Low        |
| 50 – 79.99        | Medium     |
| Below 50          | High       |

---

## System Architecture

```text
                    VRIP PLATFORM
                         |
          +--------------+--------------+
          |                             |
      Angular                       FastAPI
      Frontend                      Backend
          |                             |
          |                       REST APIs
          |                             |
          +-------------+---------------+
                        |
                    PostgreSQL
                     Database
```

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
│   │
│   ├── package.json
│   └── angular.json
│
├── .gitignore
└── README.md
```

---

## Installation & Setup

### Prerequisites

Install the following software before running the project:

* Python 3.12+
* Node.js
* Angular CLI
* PostgreSQL
* Git

---

## Backend Setup

Open a terminal and navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start the FastAPI server:

```bash
python -m uvicorn app.main:app --reload
```

Backend URL:

```text
http://127.0.0.1:8000
```

API documentation:

```text
http://127.0.0.1:8000/docs
```

---

## Frontend Setup

Open another terminal and navigate to the frontend:

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

Frontend URL:

```text
http://localhost:4200
```

---

## Application Modules

```text
Login / Registration
        ↓
Dashboard
        ↓
Vendor Management
        ↓
Vendor Reliability & Risk
        ↓
Procurement Management
        ↓
Purchase Orders
        ↓
Performance & Compliance
        ↓
Reports & Analytics
        ↓
Notifications & Audit Logs
        ↓
Supply Chain Analytics
```

---

## Security

The application includes:

* JWT-based authentication
* Protected API endpoints
* Role-Based Access Control
* Angular route guards
* HTTP authentication interceptor
* Secure password authentication
* User authorization

---

## Reporting & Analytics

The platform provides analytical information for:

* Total vendors
* Vendor risk levels
* Procurement activities
* Purchase orders
* Vendor performance
* Compliance
* Order status
* Supplier performance
* Defective units
* Supply-chain activities

Reports can also be exported for further analysis.

---

## Future Enhancements

* Cloud deployment
* AI-based vendor risk prediction
* Predictive procurement analytics
* Automated email notifications
* Advanced supplier forecasting
* ERP system integration
* Mobile application
* Advanced business intelligence dashboards

---

## Repository

**GitHub Repository:**

https://github.com/Hrishi18162/VRIP-Vendor-Reliability-Intelligence-Platform

---

## Author

**Hrishitha Kotte**

**Project:** Vendor Reliability Intelligence Platform (VRIP)

**Technology:** Angular + FastAPI + PostgreSQL

**Project Type:** Full-Stack Web Application
