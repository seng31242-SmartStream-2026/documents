# SmartStream: High-Level Architecture & Technology Stack

## 1. Architectural Pattern

SmartStream operates on a **Client-Server Architecture** utilizing the **MVC (Model-View-Controller)** design pattern. To streamline development and deployment, the system is designed as a single, highly **mobile-responsive web application** rather than maintaining separate desktop and native mobile codebases.

This approach enables:

* **Directors and Accountants** to access comprehensive dashboards and reports using desktop or laptop computers.
* **Distributors** to use a streamlined, touch-friendly interface on smartphones and tablets.
* Easy deployment and maintenance through a single codebase.
* Consistent user experience across all devices and platforms.

---

## 2. High-Level Architecture

The SmartStream system consists of four main layers:

### 2.1 Client Layer (Frontend)

**Technology:** React with TypeScript

The frontend provides the user interface through a web browser. It is responsible for:

* Displaying dashboards and reports.
* Managing inventory and order information.
* Capturing and uploading invoice images.
* Providing responsive layouts for desktop and mobile users.
* Communicating with backend APIs.

### Users

* Directors
* Accountants
* Distributors

---

### 2.2 Application Layer (Backend)

**Technology:** Node.js with Express

The backend serves as the application's controller layer and handles:

* User authentication and authorization.
* Business logic processing.
* Order management.
* Inventory management.
* OCR processing workflows.
* Communication with the database and cloud storage.

The backend exposes RESTful APIs that are consumed by the React frontend.

---

### 2.3 Data Layer

**Technology:** PostgreSQL

PostgreSQL is used as the primary relational database management system.

It stores:

* User accounts
* Product information
* Inventory records
* Orders and deliveries
* Financial transactions
* OCR extracted data
* System logs and audit records

PostgreSQL ensures:

* Data integrity
* ACID compliance
* Reliable transaction processing
* Efficient querying and reporting

---

### 2.4 Storage Layer

**Technology:** AWS S3

AWS S3 is used for storing large files that should not be kept directly in the database.

Examples include:

* Invoice images
* Product photographs
* Delivery proof images
* OCR source documents
* Generated reports

Benefits include:

* High scalability
* High availability
* Secure storage
* Cost-effective file management

---

## 3. Technology Stack Justification

### Frontend: React + TypeScript

#### Justification

* Component-based architecture promotes code reusability.
* TypeScript provides strong type checking and improved maintainability.
* Excellent support for responsive web applications.
* Large ecosystem and community support.
* Faster development through reusable UI components.

---

### Backend: Node.js + Express

#### Justification

* High-performance asynchronous architecture.
* Efficient handling of multiple concurrent users.
* Lightweight and scalable framework.
* Easy integration with frontend technologies.
* Strong support for RESTful API development.

---

### Database: PostgreSQL

#### Justification

* Reliable relational database management system.
* Strong data consistency and integrity.
* Excellent support for complex queries.
* Suitable for inventory, finance, and transactional systems.
* Open-source and highly scalable.

---

### Storage: AWS S3

#### Justification

* Designed for large-scale file storage.
* High durability and availability.
* Secure cloud-based storage solution.
* Supports image and document management requirements.
* Reduces database storage overhead.

---

## 4. System Benefits

The selected architecture provides:

* Scalability for future growth.
* High maintainability through MVC separation.
* Responsive access across desktop and mobile devices.
* Secure and reliable data management.
* Efficient handling of large media files.
* Simplified deployment and maintenance through a single web application.

---

## 5. Summary

This PR introduces the High-Level Architecture and Technology Stack Justification for the Software Design Specification (SDS). It updates our architectural approach to reflect a single mobile-responsive web application rather than separate native builds.
