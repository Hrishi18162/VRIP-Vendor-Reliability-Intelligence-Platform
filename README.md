
# VRIP - Vendor Reliability Intelligence Platform

A full-stack vendor reliability and procurement management platform designed to help organizations monitor vendor performance, assess supplier risk, manage procurement operations, and gain actionable supply-chain insights.

---

## Project Overview

**Vendor Reliability Intelligence Platform (VRIP)** is a full-stack web application developed using **Angular, FastAPI, and PostgreSQL**.

The platform centralizes vendor management, procurement, purchase orders, vendor performance, reliability scoring, risk assessment, contracts, compliance, notifications, reporting, and supply-chain analytics in a single system.

VRIP helps organizations monitor supplier performance and use structured data to support procurement and vendor-management activities.

---

## Objectives

* Centralize vendor and procurement information.
* Monitor vendor performance and reliability.
* Calculate vendor reliability scores.
* Classify vendors according to risk levels.
* Manage procurement requests and purchase orders.
* Monitor vendor compliance and contracts.
* Provide dashboards and analytical insights.
* Generate reports and export business data.
* Maintain notifications and audit records.
* Analyze supply-chain and procurement data.

---

## Key Features

### Authentication and Authorization

* User registration and login.
* JWT-based authentication.
* Role-based access control.
* Protected frontend routes.
* Authorized backend API access.

### Vendor Management

* Vendor registration and management.
* Vendor contact and business information.
* Vendor performance monitoring.
* Vendor reliability scoring.
* Risk-level classification.
* Vendor status tracking.

### Procurement Management

* Procurement request creation and management.
* Procurement status tracking.
* Vendor association.
* Budget and quantity management.

### Purchase Order Management

* Purchase order creation and management.
* Vendor and procurement association.
* Order status tracking.
* Order amount and delivery information.
* Defective-unit tracking.
* Compliance information.

### Vendor Performance and Risk Assessment

VRIP evaluates vendors using four major performance parameters:

* Delivery Score
* Quality Score
* Payment Score
* Compliance Score

The platform calculates an overall reliability score based on these parameters and assigns an appropriate risk level.

### Contracts and Compliance

* Contract management.
* Compliance monitoring.
* Vendor compliance tracking.
* Contract information management.

### Notifications and Audit Logs

* System activity notifications.
* Risk warnings.
* Operational alerts.
* Audit log tracking.
* Activity monitoring.

### Reports and Analytics

* Vendor reports.
* Procurement reports.
* Performance analytics.
* Dashboard statistics.
* Data export.
* Supply-chain analytics.

### Supply Chain Analytics

The platform provides analytical insights into:

* Order status.
* Supplier performance.
* Product and category distribution.
* Compliance.
* Defective units.
* Procurement value.

---

## Technology Stack

| Layer             | Technologies                     |
| ----------------- | -------------------------------- |
| Frontend          | Angular, TypeScript, HTML5, CSS3 |
| Visualization     | Chart.js                         |
| Backend           | Python, FastAPI                  |
| ORM               | SQLAlchemy                       |
| Authentication    | JWT                              |
| Authorization     | Role-Based Access Control        |
| Database          | PostgreSQL                       |
| Reporting         | ReportLab                        |
| Data Export       | OpenPyXL                         |
| API Documentation | Swagger / OpenAPI                |
| Version Control   | Git and GitHub                   |

---

## Vendor Reliability Scoring

VRIP evaluates vendor reliability using four performance factors:

| Parameter        | Description                            |
| ---------------- | -------------------------------------- |
| Delivery Score   | Evaluates delivery performance         |
| Quality Score    | Evaluates product or service quality   |
| Payment Score    | Evaluates payment-related performance  |
| Compliance Score | Evaluates compliance with requirements |

The overall reliability score is calculated as the average of these four performance scores.

### Risk Classification

| Reliability Score | Risk Level |
| ----------------: | ---------- |
|          80 - 100 | Low        |
|        50 - 79.99 | Medium     |
|          Below 50 | High       |

This classification allows organizations to identify vendors that may require additional monitoring.

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
       Vendors       Procurement     Analytics
          |              |               |
   Vendor Risk      Purchase Orders   Reports
                                      |
                               Supply Chain
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

## Application Modules

The platform is organized into the following major modules:

1. **Authentication**
2. **Dashboard**
3. **Vendor Management**
4. **Procurement Management**
5. **Purchase Order Management**
6. **Vendor Performance**
7. **Risk Assessment**
8. **Contracts and Compliance**
9. **Notifications**
10. **Audit Logs**
11. **Reports**
12. **Analytics**
13. **Supply Chain Analytics**

---

## Application Workflow

```text
User
 |
 v
Authentication
 |
 v
Dashboard
 |
 +-------------------+
 |                   |
 v                   v
Vendors          Procurement
 |                   |
 v                   v
Risk Assessment   Purchase Orders
 |                   |
 +---------+---------+
           |
           v
    Performance Analytics
           |
           v
      Reports & Exports
           |
           v
 Notifications & Audit Logs
           |
           v
   Supply Chain Insights
```

---

## Installation and Setup

### Prerequisites

Install the following before running the project:

* Python 3.12+
* Node.js
* Angular CLI
* PostgreSQL
* Git
* Visual Studio Code

---

## Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```powershell
venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Configure the PostgreSQL database and required environment variables.

Start the FastAPI server:

```bash
python -m uvicorn app.main:app --reload
```

Backend URL:

```text
http://127.0.0.1:8000
```

### API Documentation

Swagger API documentation:

```text
http://127.0.0.1:8000/docs
```

---

## Frontend Setup

Open a new terminal and navigate to the frontend:

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

## Security

The application includes:

* JWT-based authentication.
* Role-based authorization.
* Protected Angular routes.
* HTTP authorization interceptors.
* Backend API authorization.
* Restricted access to protected operations.

Sensitive configuration values should be stored in environment variables and should not be committed to the repository.

---

## Reporting and Analytics

VRIP provides reporting and analytics for:

* Vendor reliability.
* Vendor risk levels.
* Procurement activities.
* Purchase orders.
* Vendor performance.
* Compliance.
* Supply-chain operations.
* System activities.

The platform also supports exporting selected business information for further analysis.

---

## Future Enhancements

Planned improvements may include:

* Machine-learning-based vendor risk prediction.
* Advanced supplier benchmarking.
* Automated email notifications.
* Cloud deployment.
* Docker containerization.
* Advanced procurement forecasting.
* Automated scheduled reports.
* Enhanced predictive analytics.
* Expanded supply-chain intelligence.

---

## GitHub Repository

**Repository:**
https://github.com/Hrishi18162/VRIP-Vendor-Reliability-Intelligence-Platform

---

## Author

**Hrishitha Kotte**

Full Stack Development Project
Vendor Reliability Intelligence Platform

---

## License

This project is developed for educational and project demonstration purposes.
