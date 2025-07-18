\newpage

Quality Requirements
====================
[//]: # (Nicoletta)

Quality Tree
------------

![quality_tree.png](Images/quality_tree.png)

Quality Scenarios
-----------------

**Reliability**   
A user updates their account email address. Due to a bug in the email service, the confirmation email fails to send — but the system logs the issue, queues the email for retry, and does not corrupt the user’s data or prevent further account actions.

**Security**   
A malicious actor attempts unauthorized access to customer data via a public API. The system immediately blocks the request, logs the attempt, and sends an alert to the security team within 5 minutes.

**Usability**   
A first-time user opens the app and successfully completes profile setup without external guidance, within 10 minutes, aided by intuitive navigation and contextual help prompts.
