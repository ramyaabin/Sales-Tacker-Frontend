# Sales Tracker – Sales Management System

> **Confidential Project**
>
> A full-stack MERN web application developed to digitize and streamline daily sales operations for a global accessories brand across multiple retail outlets in the UAE.
>
> Due to client confidentiality, the source code and live production website are not publicly available.

---

## 📌 Overview

**Sales Tracker** is a role-based sales management platform designed for retail sales teams and administrators.

The application replaces manual sales tracking and reporting workflows with a centralized web-based system supporting:

* Secure authentication and authorization
* Sales entry and product lookup
* Daily and monthly sales analytics
* Employee performance tracking
* Leave management and approval workflows
* Product catalogue management
* CSV and Excel reporting
* Cloud-based deployment

---

## 🛠️ Technology Stack

| Area                   | Technologies                                                    |
| ---------------------- | --------------------------------------------------------------- |
| **Frontend**           | React 18, Vite, Responsive UI                                   |
| **Backend**            | Node.js, Express.js, REST API                                   |
| **Database**           | MongoDB Atlas                                                   |
| **Authentication**     | JWT, Role-Based Access Control (RBAC), OTP-based password reset |
| **File Processing**    | Multer, SheetJS                                                 |
| **Email**              | Nodemailer, Gmail                                               |
| **Charts & Analytics** | Dashboard charts and KPI visualizations                         |
| **Deployment**         | Render                                                          |
| **Version Control**    | Git, GitHub                                                     |

---

# 👥 User Roles

## Admin Portal

Administrators have centralized control over sales operations and employee management.

### Dashboard & Analytics

* Total Revenue KPI
* Total Transactions
* Active Salesmen
* Leave Days
* Employee performance comparison
* Top 5 brands by revenue
* Performer of the Month
* Daily and monthly sales analysis

### Employee Management

* Create salesman accounts
* Delete salesman accounts
* Reset passwords
* Manage employee access through role-based permissions

### Leave Management

* View all leave applications
* Approve or reject requests
* Add rejection reasons
* Track application and action timestamps
* Download complete leave reports
* Download individual salesman leave reports

### Product Management

* Upload Excel product catalogue
* Replace the complete product catalogue
* Search products by:

  * Brand
  * Model
  * Barcode
  * Description

### Reporting

* Download sales reports as CSV
* Download leave reports as CSV
* Generate per-salesman reports
* Include outlet/location information in reports

---

# 👤 Salesman Portal

Salesmen can record daily sales and manage their own leave requests.

### Sales Entry

* Select retail outlet
* Search products by model or barcode
* Live product suggestions
* Automatic product information retrieval
* Automatic price calculation
* Quantity-based total calculation
* Product master validation

### Sales History

Salesmen can view sales records containing:

* Date
* Location
* Brand
* Barcode
* Description
* Quantity
* Price
* Total

### Sales Dashboard

* Daily sales view
* Monthly sales view
* Date-based filtering
* Sales performance overview

### Leave Management

* Submit leave applications
* Duplicate-date detection
* View leave history
* Track request status
* View rejection reasons from administrators

---

# 🔐 Authentication & Security

The application implements multiple security mechanisms:

### JWT Authentication

Secure token-based authentication for protected application routes.

### Role-Based Access Control

Separate permissions for:

* **Admin**
* **Salesman**

Administrative functionality is restricted to authorized users.

### Password Reset

Administrators can reset passwords using a **6-digit OTP** delivered to their registered email address.

OTP verification includes a **5-minute expiration period**.

### Account Management

* No public self-registration
* User accounts are created by administrators
* Protected API routes
* Role-based middleware
* Secure routing

---

# 📊 Analytics & Reporting

The platform provides management-level visibility into retail performance.

### Key Performance Indicators

* Revenue
* Transactions
* Active salesmen
* Leave days

### Visual Analytics

**Employee Performance**

Bar chart comparing sales performance across employees.

**Brand Revenue**

Pie chart displaying revenue contribution from the top five brands.

**Monthly Performance**

Highlights the highest-performing employee for the selected period.

---

# 📦 Product Catalogue

The product management module supports centralized product master management.

Products can be uploaded using Excel (`.xlsx`) files and processed using **SheetJS**.

Product information includes:

* Brand
* Model
* Barcode / EAN
* Description
* Price

The sales entry system uses this product master to validate and automatically populate product information.

---

# 📋 Leave Management Workflow

The leave management module provides a complete approval workflow:

```text
Salesman
   ↓
Submit Leave Request
   ↓
Duplicate Date Validation
   ↓
Admin Review
   ↓
┌───────────────┐
│               │
Approve       Reject
│               │
↓               ↓
Approved      Rejection Reason
```

The system maintains timestamps for application and administrative actions to provide an audit trail.

---

# ✨ Key Enhancements

The project evolved through multiple feature improvements:

* Added product description to improve product identification
* Added barcode/EAN search for faster sales entry
* Introduced complete leave management workflow
* Added timestamped leave audit trail
* Improved brand revenue visualization
* Added outlet location to sales records
* Included outlet information in CSV reports
* Integrated Sudio as an additional product brand
* Updated the product master dataset

---

# 📱 Responsive Design

The application is designed for use across different screen sizes.

The responsive interface supports:

* Desktop
* Laptop
* Tablet
* Mobile

This allows sales staff to record and review sales from different retail environments.

---

# ☁️ Deployment

The application was deployed using **Render** with separate frontend and backend services.

The deployment workflow supports:

```text
GitHub
   ↓
Automatic Deployment
   ↓
Frontend + Backend
   ↓
MongoDB Atlas
```

The application was designed for remote accessibility across retail locations.

Due to project confidentiality, the production URL is not publicly shared.

---

# ✅ Project Scope

### Included

* Responsive web application
* Secure authentication
* Role-based authorization
* Sales management
* Product master validation
* Automated sales calculations
* Leave management
* Sales analytics
* Employee management
* CSV reporting
* Excel product uploads
* Cloud deployment

### Not Included

* Payment gateway
* Public customer access
* Profit/margin analytics
* Inventory stock deduction
* ERP integration
* Multi-company database separation

---

# 💡 Skills Demonstrated

This project demonstrates practical experience with:

**Frontend Development**

* React
* Vite
* Responsive UI
* Dynamic dashboards
* Form handling

**Backend Development**

* Node.js
* Express.js
* REST APIs
* Middleware
* Authentication
* Authorization

**Database**

* MongoDB
* MongoDB Atlas
* Data modelling

**Security**

* JWT
* RBAC
* OTP authentication
* Protected routes

**Data & Reporting**

* Excel processing
* CSV generation
* Dashboard analytics
* Data visualization

**Deployment**

* GitHub
* Render
* Cloud database integration

---

## 📈 Business Impact

The system was designed to centralize retail sales operations, reduce manual data entry, improve product identification, simplify leave management, and provide administrators with consolidated sales and employee performance information.

---

## 🔒 Confidentiality Notice

This project was developed for a business client and contains confidential business workflows and data.

Therefore:

* Source code is not publicly available
* Production URL is not publicly shared
* Client-specific data has not been published
* Screenshots or demonstrations can be provided privately where appropriate

The project description is provided to demonstrate the technical architecture, development responsibilities, and skills involved without exposing confidential information.
