# User Management System

A simple Spring Boot-based backend application that allows for managing user data including names and membership types. This project is API-first, meaning all functionality is exposed through REST endpoints and is documented using Swagger (OpenAPI). No frontend is used.

---

## 🚀 Features

- Create a new user (POST)
- Fetch all users (GET)
- Fetch a user by ID (GET)
- Delete a user by ID (DELETE)
- Uses an in-memory H2 database for testing
- Swagger UI integration for easy API testing
- Fully Java-based backend using Spring Boot 3.5.3
- Organized in a clean MVC architecture

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot 3.5.3
- Spring Data JPA
- H2 in-memory database
- Lombok
- Swagger/OpenAPI (via Springdoc)
- Maven for build and dependency management

---

## 🗂️ Project Structure

com.example.membership
├── controller # REST API endpoints
├── model # User entity/model
├── repository # JPA repository interface
├── service # Business logic layer
└── UserManagementManagerApplication.java # Main application


---

## 📦 Setup Instructions

### Prerequisites

- Java 17 or later installed
- IntelliJ IDEA or any Java IDE
- Maven installed and configured
- Git installed (optional, for pushing to GitHub)

### Steps

1. Clone the repo (or create your own via IntelliJ)
2. Add the required dependencies:
   - Spring Web
   - Spring Data JPA
   - H2 Database
   - Lombok
   - Springdoc OpenAPI UI (for Swagger)
3. Run the application via:
   - `UserManagementManagerApplication.java` (green run button)

---

## 🌐 Accessing the Application

### Swagger UI

To test all APIs visually using Swagger:

http://localhost:8080/swagger-ui/index.html


You can try all endpoints directly from this interface.

---

## 📋 API Endpoints

| Method | Endpoint           | Description             |
|--------|--------------------|-------------------------|
| POST   | `/users`           | Add a new user          |
| GET    | `/users`           | Get all users           |
| GET    | `/users/{id}`      | Get user by ID          |
| DELETE | `/users/{id}`      | Delete user by ID       |

> Note: ID is auto-generated by the system.

---

## 🧪 Sample JSON for POST Request

json:
{
  "name": "Alice",
  "membership": "GOLD"
}

Do not include the id field in POST requests, as it is auto-generated.

H2 Database Console: http://localhost:8080/h2-console

✅ Running Notes
Once the application is started, it keeps running and listening on port 8080 until stopped.

You only need to restart if you change code or configuration files.

🔐 Future Enhancements
Add validation using Hibernate Validator

Integrate authentication & authorization

Switch to a persistent database like MySQL or PostgreSQL

Add a React or Angular frontend

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📄 License
This project is licensed under the MIT License.

👤 Author
Kabir Sheikh

Let me know how you liked the backend application and feel free to reach out if you have any questions!
