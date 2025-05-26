# Solution Strategies
## Crosscutting Concepts
**Development concepts**
* Component-based architecture using microservices 

**Architecture and design patterns**
* Model-View-Controller
* Event-driven architecture

**Safety and security concepts**
* JWT-based authentication and role-based access control
* Data validation and input sanitation

## Decisions
| Context                                                                                                                                     | Decision                                                                  | Consequences                                                                                                                             |
|---------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| We need to secure communication and manage user sessions across mobile and backend.                                                         | We will implement JWT-based authentication and role-based access control. | Improves security and enables scalable session handling, but requires careful token management and role definition.                      |
| We need scalable and independently deployable components for each service (e.g. ride handling, user profile, payments).                     | We will use a microservices architecture.                                 | Each service can be developed and scaled independently, but requires DevOps setup, inter-service communication, and monitoring overhead. |
| Deploy on cloud infrastructure (e.g. AWS)We want to maintain a clean separation between front-end logic, backend services, and data access. | We will use the Model-View-Controller (MVC) pattern.                      | Code will be more maintainable and testable, but may require stricter discipline in structuring features.                                |
