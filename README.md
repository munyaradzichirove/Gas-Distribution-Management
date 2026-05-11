### Gas

This is an app for managing gas business

### Installation

You can install this app using the [bench](https://github.com/frappe/bench) CLI:

```bash
cd $PATH_TO_YOUR_BENCH
bench get-app $URL_OF_THIS_REPO --branch develop
bench install-app gas
```

### Contributing

This app uses `pre-commit` for code formatting and linting. Please [install pre-commit](https://pre-commit.com/#installation) and enable it for this repository:

```bash
cd apps/gas
pre-commit install
```

Pre-commit is configured to use the following tools for checking and formatting your code:

- ruff
- eslint
- prettier
- pyupgrade

### License

mit
# Gas-Distribution-Management
📦 Gas Distribution Management System

A Frappe/ERPNext-based system for managing gas distribution operations including customer requests, bulk supply, cylinder tracking, approvals, quotations, deliveries, and lifecycle management.

🚀 Overview

This system streamlines gas supply operations for both retail customers and bulk distributors. It centralizes:

Customer gas requests
Internal approvals
Quotation generation
Sales orders and delivery
Cylinder exchange & refill tracking
Warehouse stock management

Built on Frappe Framework
 / ERPNext, it leverages existing ERP capabilities with custom workflows for gas distribution workflows.

🧠 Core Concept

Everything starts from a single entry point:

Gas Request

This represents any demand for gas (refill, exchange, or bulk supply), regardless of customer type.

🔄 System Workflow
Gas Request
→ Internal Approval
→ Quotation
→ Customer Acceptance
→ Sales Order
→ Delivery Note
→ Invoice
👥 User Roles
Customer / Distributor
Submits gas requests via portal
Sales/Admin
Reviews requests
Sets pricing logic
Generates quotations
Warehouse Team
Manages stock
Dispatches cylinders
Delivery Engineer
Handles delivery and cylinder swaps
Logs service completion
📄 Key Features
🟢 Gas Request Management
Unified request system for retail + bulk customers
Request types: Refill, Exchange, Bulk Supply
Status tracking & workflow automation
🟡 Approval System
Internal approval before quotation
Role-based workflow routing
🟠 Quotation Management
Automated quotation generation
Pricing logic: Standard / Contract / Negotiated
PDF sharing with customers
🔵 Inventory & Cylinder Tracking
Warehouse stock control
Serial number tracking for cylinders
Exchange and refill lifecycle support
🔴 Delivery Operations
Delivery Notes for dispatch
Task assignment for field engineers
Real-time stock updates
🏗️ Tech Stack
Frappe Framework
ERPNext (core modules)
Python (backend logic)
MariaDB / MySQL
Redis (background jobs)
JavaScript (UI customization)
📊 Data Model (Core Doctypes)
Gas Request (Custom)
Customer 
Item 
Warehouse 
Serial No 
Quotation 
Sales Order 
Delivery Note 
⚙️ Installation (Dev Setup)
bench get-app gas_system
bench --site your-site.local install-app gas_system
bench start
🎯 Goal of This Project

To build a real-world gas distribution ERP layer that:

Reduces cylinder loss
Automates approvals & pricing
Tracks full lifecycle of gas containers
Improves operational efficiency across warehouses & distributors
📌 Future Enhancements
QR code cylinder tracking
Mobile delivery app
GPS dispatch tracking
Smart pricing engine
Analytics dashboard (stock + sales + logistics)
🧑‍💻 Author

Built by Munyaradzi Chirove
ERPNext / Infrastructure / Systems Engineering enthusiast