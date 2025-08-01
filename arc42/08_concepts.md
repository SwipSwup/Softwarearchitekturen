﻿\newpage

Cross-cutting Concepts
======================
[//]: # (Ivo)
Component-based Microservice Architecture
-------------------
Our system is structured using a component-based approach with microservices. This promotes loose coupling, independent scalability, and easier development. Each service encapsulates a specific business capability and can be deployed independently, supporting team autonomy and fault isolation.

Model-View-Controller (MVC)
-------------------
We use the MVC pattern to separate user interface, business logic, and data handling across both the frontend and backend layers. This increases maintainability and testability by keeping concerns cleanly divided and responsibilities clearly assigned.

Event-driven Architecture
-------------------
For internal communication and workflow orchestration (e.g. ride matching and notifications), we implement event-driven architecture using asynchronous messaging. This helps decouple services, improves scalability, and allows the system to react in near real-time.

JWT Authentication and RBAC
-------------------
Security is enforced using JWT (JSON Web Token) for stateless authentication across services. Role-based access control (RBAC) is used to restrict access to protected resources, depending on whether the user is a driver, rider, or admin.

Input Validation and Sanitization
-------------------
To prevent common vulnerabilities such as injection attacks or malformed input, we apply strict validation rules and sanitize all incoming data at the controller level. This protects internal services and the database layer from untrusted input.

