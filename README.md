# Task Manager Application  

A simple Spring Boot application for managing tasks, built with Spring Data JPA and MySQL.  

## Features  
- Create, update, delete, and view tasks  
- RESTful API built with **Spring Boot Web**  
- Persistence with **Spring Data JPA** and **MySQL**  
- Unit testing with **Spring Boot Starter Test**  

## Tech Stack  
- Java 17  
- Spring Boot 3.5.4  
- Spring Data JPA  
- Spring Web  
- MySQL (with MySQL Connector/J)  

## Getting Started  

### Prerequisites  
- Java 17+  
- Maven 3+  
- MySQL  

### Setup  
1. Clone the repository:  
   ```bash
   git clone https://github.com/Tharun-0408/task-manager.git
   cd task-manager/todo

2. Configure your MySQL database in application.properties
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
   spring.datasource.username=your-username
   spring.datasource.password=your-password
   spring.jpa.hibernate.ddl-auto=update
   
3. Open the todo folder directly in IntelliJ IDEA (or your preferred IDE). IntelliJ will automatically detect it as a Maven project.
   
4. Build and run the application
   ```bash
   mvn spring-boot:run

## API Endpoints

### Tasks
- `GET /tasks` → Get all tasks  
- `GET /tasks/{id}` → Get a task by ID  
- `POST /tasks` → Create a new task  
- `PUT /tasks/{id}` → Update a task  
- `DELETE /tasks/{id}` → Delete a task

  ### Example Request Bodies  (for testing in Postman or curl)

#### Create a Task (POST /tasks)  
```json
{
  "title": "Finish project",
  "description": "Complete the Spring Boot task manager",
  "completed": false
}
```
#### Update a Task (PUT /tasks/{id})
```json
{
  "title": "Finish project",
  "description": "Add README improvements and push to github",
  "completed": true
}
```





   
