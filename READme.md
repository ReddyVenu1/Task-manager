# Task Manager - Spring Boot Application

## 📌 Overview
A web-based Task Manager built using **Spring Boot**. This application provides REST APIs to create, update, view, and delete tasks, demonstrating the use of Spring Boot, Spring Data JPA, and a relational database for persistent storage.

## 🛠 Technologies Used
- Java
- Spring Boot
- Spring Data JPA (Hibernate)
- MySQL (or H2 for in-memory testing)
- Maven

## 🚀 Features
- Add new tasks with title, description, and due date
- View all tasks or a specific task by ID
- Update task details
- Mark tasks as completed
- Delete tasks
- Persistent storage using MySQL/H2

## 🗂 Project Structure
```
src/
 ├── main/java/com/example/taskmanager
 │     ├── controller   # REST controllers
 │     ├── model        # Entity classes
 │     ├── repository   # JPA repositories
 │     └── service      # Business logic
 └── main/resources
       ├── application.properties
       └── schema.sql / data.sql (if needed)
```

## ⚙️ Setup & Run
1. Clone the repository:
```bash
git clone <your-repo-link>
cd task-manager
```
2. Configure your database in `application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/taskdb
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```
3. Build and run the project:
```bash
mvn spring-boot:run
```

## 📍 API Endpoints
- `POST /tasks` → Create a new task  
- `GET /tasks` → Get all tasks  
- `GET /tasks/{id}` → Get task by ID  
- `PUT /tasks/{id}` → Update a task  
- `DELETE /tasks/{id}` → Delete a task  

---

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).
