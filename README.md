# Dorm App

A dormitory management system built with **Spring Boot** and **Angular** to facilitate student room assignments and administration.

## Features
- User authentication and role-based access control (Students & Wardens)
- Student registration and profile management
- Room assignment and unassignment
- Soft and hard delete functionality for students
- API documentation with Swagger

## Tech Stack
- **Backend:** Spring Boot (Java), Spring Security, MySQL
- **Frontend:** Angular 18, Bootstrap
- **API Documentation:** Springdoc OpenAPI (Swagger)
- **Build Tools:** Gradle

## Setup & Installation

### Backend (Spring Boot)
1. Clone the repository:
   ```sh
   git clone https://github.com/ntsaousis/cf-dormapp.git
   cd cf-final-project
   ```
2. Configure **MySQL Database**:
   - Update `src/main/resources/application.properties` with your MySQL credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/dorm_db
     spring.datasource.username=root
     spring.datasource.password=your_password
     spring.jpa.hibernate.ddl-auto=update
     ```
3. Run the application:
   ```cmd
   ./gradlew bootRun
   ```
4.Populate rooms by executing `rooms.sql` manually in MySQL or enable auto-insertion.

### Frontend (Angular)
1. Navigate to the frontend directory:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the Angular development server:
   ```sh
   ng serve
   ```

## API Documentation
Once the backend is running, visit:
- Swagger UI: [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

## Deployment
- **Backend:** Can be packaged into a JAR using `./gradlew build` and deployed to a server.
- **Frontend:** Can be built with `ng build` and hosted on any static file server.

## To-Do
- Implement better UI styling
- Optimize database queries
- Add complaints and requests management.

---
### Author
Developed by **ntsaousis** for AUEB Coding Factory 6  final project.
