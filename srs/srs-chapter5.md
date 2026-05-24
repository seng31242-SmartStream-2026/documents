# Chapter 5: Non-Functional Requirements

This section specifies the non-functional requirements (quality attributes) that the SmartStream system must adhere to in order to ensure security, usability, and stability.

## 5.1 Performance

- The AI OCR processing of an invoice image shall not exceed 5 seconds under standard network conditions.
- Dashboard analytics must load within 3 seconds.

## 5.2 Security

- All user passwords must be hashed using bcrypt.
- Data in transit must be encrypted via TLS 1.2 or higher.
- The system must adhere to standard data privacy practices.

## 5.3 Usability

- The mobile application UI must be accessible and intuitive.
- The system shall require no more than 3 taps for a distributor to upload an invoice.

## 5.4 Reliability

- The system shall maintain an overall uptime of 99.9%.
- In the event of a server failure, the cloud disaster recovery protocol must allow full system restoration within 4 hours.

## 5.5 Scalability

- The cloud backend (e.g., Node.js/Spring Boot) must support automatic scaling to accommodate up to 500 concurrent distributor requests.

## 5.6 Maintainability

- The system architecture will utilize a modular, decoupled approach (e.g., React frontend, separate REST API backend).
- This architecture must allow for isolated module updates without necessitating full system downtime.
