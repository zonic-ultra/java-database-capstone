This Spring Boot application uses both MVC and REST controllers. Thymeleaf templates are used for the Admin and Doctor dashboards, while REST APIs serve all other modules. The application interacts with two databases—MySQL (for patient, doctor, appointment, and admin data) and MongoDB (for prescriptions). All controllers route requests through a common service layer, which in turn delegates to the appropriate repositories. MySQL uses JPA entities while MongoDB uses document models.

1. A user accesses the system either through the Thymeleaf-based Admin/Doctor dashboards or through REST API clients such as the Appointment or Patient modules.
2. The user’s action or request is routed to the appropriate controller: Thymeleaf Controllers for server-rendered HTML views, or REST Controllers for JSON-based API requests.
3. The controller validates the request and forwards it to the Service Layer for further processing.
4. The Service Layer applies business rules, coordinates workflows (e.g., checking doctor availability), and decides which repository should be used.
5. The Service Layer calls the Repository Layer, which communicates with either MySQL (for structured data like patient and appointment records) or MongoDB (for flexible prescription data).
6. The repositories retrieve or persist the data and return it as model objects (JPA entities for MySQL or document models for MongoDB).
7. The controller uses these models to send back the response—either rendering a Thymeleaf HTML page or returning JSON data to the client.

9. <img width="1405" height="813" alt="architecture-diagram" src="https://github.com/user-attachments/assets/aeadf53d-6b2d-4d7e-a121-12891b414cd0" />
