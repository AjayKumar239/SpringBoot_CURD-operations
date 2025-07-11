🚀 Features
Add a new student (POST)

Get all students (GET)

Get a student by ID (GET)

Update student info (PUT)

Delete a student (DELETE)

🔧 Technologies Used
Java 17+ (or your version)

Spring Boot

Spring Data JPA

MySQL or H2 Database

Maven or Gradle

Postman (for API testing)

⚙️ Setup Instructions
Clone the repository



properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/yourdbname
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
💡 You can switch to H2 for testing:

properties
Copy
Edit
spring.datasource.url=jdbc:h2:mem:testdb
spring.h2.console.enabled=true
spring.jpa.hibernate.ddl-auto=create
Run the application

bash
Copy
Edit
./mvnw spring-boot:run
Access API endpoints using Postman or browser:

POST /api/student

GET /api/student

GET /api/student/{id}

PUT /api/student/{id}

DELETE /api/student/{id}

📬 Sample JSON for POST/PUT
json
Copy
Edit
{
  "name": "John Doe",
  "email": "john@example.com",
  "address": "New York"
}
