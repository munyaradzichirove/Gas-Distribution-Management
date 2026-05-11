# 📦 Gas Distribution Management System

A Frappe/ERPNext-based system for managing gas distribution operations including customer requests, approvals, quotations, deliveries, and cylinder lifecycle tracking.

---

# 🔄 System Workflow

```text
Gas Request
→ Internal Approval
→ Quotation
→ Customer Acceptance
→ Sales Order
→ Delivery Note
→ Invoice
```

---

# 👥 User Roles

## Customer / Distributor

* Submits gas requests via portal

## Sales / Admin

* Reviews requests
* Sets pricing logic
* Generates quotations

## Warehouse Team

* Manages stock
* Dispatches cylinders

## Delivery Engineer

* Handles delivery and cylinder swaps
* Logs service completion

---

# 📄 Key Features

## 🟢 Gas Request Management

* Unified request system for retail and bulk customers
* Request types: Refill, Exchange, Bulk Supply
* Status tracking and workflow automation

---

## 🟡 Approval System

* Internal approval before quotation
* Role-based workflow routing

---

## 🟠 Quotation Management

* Automated quotation generation
* Pricing logic: Standard / Contract / Negotiated
* PDF sharing with customers

---

## 🔵 Inventory & Cylinder Tracking

* Warehouse stock control
* Serial number tracking for cylinders
* Full refill and exchange lifecycle support

---

## 🔴 Delivery Operations

* Delivery Notes for dispatch
* Task assignment for field engineers
* Real-time stock updates

---

# 🏗️ Tech Stack

* Frappe Framework
* ERPNext Core Modules
* Python (Backend Logic)
* MariaDB / MySQL
* Redis (Background Jobs)
* JavaScript (UI Customization)

---

# 📊 Data Model (Core Doctypes)

* Gas Request (Custom)
* Customer
* Item
* Warehouse
* Serial No
* Quotation
* Sales Order
* Delivery Note

---

# ⚙️ Installation (Development Setup)

```bash
bench get-app gas_system
bench --site your-site.local install-app gas_system
bench start
```

---

# 🎯 Project Goal

To build a real-world gas distribution ERP layer that:

* Reduces cylinder loss
* Automates approvals and pricing
* Tracks full lifecycle of gas containers
* Improves operational efficiency across warehouses and distributors

---

# 📌 Future Enhancements

* QR code cylinder tracking
* Mobile delivery app
* GPS dispatch tracking
* Smart pricing engine
* Analytics dashboard (stock, sales, logistics)

---

# 🧑‍💻 Author

Built by **Munyaradzi Chirove**
ERPNext • Infrastructure • Systems Engineering Enthusiast
