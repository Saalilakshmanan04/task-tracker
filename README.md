⚙️ Task Tracker – Backend (Spring Boot + MySQL)
A robust and fully functional Task Tracker Backend API built using Spring Boot, Spring Data JPA, and MySQL.
This backend powers the Task Tracker frontend by providing secure, fast, and reliable REST API endpoints.
It supports creating, updating, retrieving, and deleting tasks with full database persistence.
Designed using clean architecture principles and follows Spring Boot best practices.

📘 Project Description
This Spring Boot backend provides RESTful APIs for the Task Tracker application.
It handles all the task operations including add, fetch, update, and delete, with complete database storage using MySQL.
The backend is built using layered architecture (Controller → Service → Repository) and ensures clean separation of concerns.
It works seamlessly with the HTML/CSS/JS frontend by exposing secure endpoints.

🚀 Features

🗂 Create, Read, Update, Delete (CRUD) tasks

🏛 Spring MVC layered architecture

🗄 MySQL database persistence

🔁 Automatic JSON serialization/deserialization

📡 REST API endpoints for frontend integration

🪝 Repository pattern using Spring Data JPA

🌱 Easy to extend and scale

🛠 Tech Stack

☕ Java 17+

🌱 Spring Boot (Web + JPA + Validation)

🗄 MySQL Database

📦 Maven

🔗 REST API

📂 Project Structure
src/
 └── main/
     ├── java/com/project/task_tracker/
     │     ├── controller/
     │     │      └── TaskController.java
     │     ├── service/
     │     │      ├── TaskService.java
     │     │      └── TaskServiceImp.java
     │     ├── repository/
     │     │      └── TaskRepository.java
     │     ├── model/
     │     │      └── Task.java
     │     └── TaskTrackerApplication.java
     └── resources/
           ├── application.properties
           └── static/

🔧 How to Run the Backend
1️⃣ Clone the Repository
git clone https://github.com/saalilakshmanan04/task-tracker.git
cd task-tracker-backend

2️⃣ Configure MySQL in application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/taskdb
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

3️⃣ Create MySQL Database
CREATE DATABASE taskdb;

4️⃣ Run the Application

Using IntelliJ IDEA or:

mvn spring-boot:run

5️⃣ Backend will start at:
http://localhost:8080

📡 API Endpoints
🔹 Get All Tasks
GET /api/tasks

🔹 Create Task
POST /api/tasks

🔹 Delete Task
DELETE /api/tasks/{id}

🔹 Update Task Status / Full Update
PUT /api/tasks/{id}

🧠 Architecture Overview

Controller → Handles HTTP requests

Service → Business logic

Repository → Database operations using Spring Data JPA

Model → Entity class mapped to MySQL table

This clean separation allows easy maintenance and future scalability.
