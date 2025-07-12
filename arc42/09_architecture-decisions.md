\newpage

Cross-cutting Concepts
======================
[//]: # (Nicoletta)
| Problem                                                                     | Considered Alternatives                                      | Decision                                                                                                         |
|-----------------------------------------------------------------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| How to implement real-time communication between rider and driver           | 1. REST API polling<br>2. WebSockets<br>3. Realtime Database | Use WebSockets for bi-directional communication to support live ride status updates and driver location tracking |
| How to scale the system to handle sudden demand spikes (e.g. during events) | 1. Manually scale servers<br>2. Use Docker with Kubernetes   | Chose Kubernetes for better control and autoscaling                                                              |
| How to store and manage geolocation data efficiently                        | 1. Relational DB with spatial extension (PostGIS)            | Decided on PostgreSQL with PostGIS for reliable geospatial queries                                               |
