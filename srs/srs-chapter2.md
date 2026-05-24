# Chapter 2: Overall Description

## 2.1 Product Perspective

SmartStream is an independent, custom-built software platform designed to operate as the centralized management ecosystem for KTD Lanka's distribution operations. It serves as a direct replacement for the current disconnected manual systems (Microsoft Excel and paper invoices) which are prone to duplication and human error. The system interfaces with third-party Email and SMS API gateways to dispatch automated stock alerts and utilizes secure cloud architecture to guarantee data availability and disaster recovery.

## 2.2 User Classes and Characteristics

The system implements strict Role-Based Access Control (RBAC) to support the following identified actors:

- **Director / Executive:** Requires strategic oversight. Needs a remote dashboard for real-time monitoring of company performance, sales analytics, and high-level reports across all locations.
- **Manager / Accountant:** Responsible for daily operational and financial management. Requires automated financial tools and easy invoice generation workflows.
- **Inventory Staff:** Manages physical warehouse operations for large quantities of imported goods (e.g., Korean ramen, Baskin Robbins). Needs quick access to update stock levels and relies on automated low-stock alerts.
- **Distributors:** Handles external supply chain logistics. Benefits from instant messaging and real-time updates regarding supply chain movements.

## 2.3 Operating Environment

- **Frontend:** A responsive web application built with React, accessible via standard web browsers (Chrome, Edge, Safari) on both desktop and mobile devices.
- **Backend:** A robust REST API powered by Node.js, managing server logic and request handling.
- **Database:** A NoSQL database utilizing MongoDB to store scalable and flexible data structures for inventory and invoices.
- **Hosting / Infrastructure:** Deployed on a highly available cloud environment to support the mandatory disaster recovery requirements.

## 2.4 Design and Implementation Constraints

- **Timeline Constraint:** The project must adhere to a strict 8-week Design Phase, followed by a 4-month Development Phase, and a 1-month Testing & Deployment Phase.
- **Security Constraint:** Because the system handles sensitive financial and business data, it must enforce granular role-based access to prevent Inventory Staff from accessing Managerial financial tools, and vice versa.
- **Redundancy Constraint:** The client explicitly mandates a cloud-based disaster recovery solution; therefore, the architecture must support automated secure document backups.

## 2.5 Assumptions and Dependencies

- **Internet Availability:** It is assumed that KTD Lanka's offices and key personnel have consistent internet access to connect to the cloud-based system.
- **Third-Party Services:** The automated low-stock alerts depend on the continuous availability and uptime of third-party Email and SMS service providers.
- **Client Engagement:** It is assumed the client will remain actively available for the duration of the design and development phases for user acceptance testing and feedback.

---
