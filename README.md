# 🎓 Student Management System

A robust **Student Management System** built using **Spring Boot, Spring Data JPA, and MySQL** that allows administrators to manage student records efficiently.

## 🚀 Features

* ➕ Add new student records
* 📋 View all students with pagination
* 🔍 Search students by name, department, and course
* ✏️ Update student information
* 🗑️ Delete student records
* 🔐 Admin Login Authentication
* 📊 Dashboard Statistics
* ⚠️ Global Exception Handling
* 📱 RESTful API Design
* 🏗️ Layered Project Architecture

---

## 🛠️ Tech Stack

* Java 17+
* Spring Boot
* Spring Data JPA
* MySQL
* Maven
* Lombok
* REST APIs
* Git & GitHub

---

## 📂 Project Structure

```text
student-management-system/
│
├── src/
│   ├── main/
│   │
│   ├── java/com/example/demo/
│   │
│   ├── config/
│   │   ├── DataInitializer.java
│   │   ├── GlobalExceptionHandler.java
│   │   └── WebConfig.java
│   │
│   ├── controller/
│   │   ├── AuthController.java
│   │   └── StudentController.java
│   │
│   ├── dto/
│   │   ├── ApiResponse.java
│   │   ├── DashboardStats.java
│   │   ├── LoginRequest.java
│   │   ├── LoginResponse.java
│   │   └── StudentRequest.java
│   │
│   ├── model/
│   │   ├── Admin.java
│   │   └── Student.java
│   │
│   ├── repository/
│   │   ├── AdminRepository.java
│   │   └── StudentRepository.java
│   │
│   ├── service/
│   │   ├── AuthService.java
│   │   └── StudentService.java
│   │
│   ├── DemoApplication.java
│   │
│   └── resources/
│       ├── static/
│       ├── templates/
│       └── application.properties
│
├── test/
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/student-management-system.git
cd student-management-system
```

### Configure Database

Create a MySQL database:

```sql
CREATE DATABASE student_management;
```

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/student_management
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

## ▶️ Run the Application

### Using Maven

```bash
mvn spring-boot:run
```

### Or

```bash
mvn clean install
java -jar target/demo.jar
```

Application will start at:

```text
http://localhost:8080
```

---

## 📸 Application Flow

```text
Admin Login
      ↓
Dashboard
      ↓
Add Student
      ↓
View Students
      ↓
Search Students
      ↓
Update Student
      ↓
Delete Student
      ↓
Dashboard Statistics Updated
```

---

## 🔗 Sample API Endpoints

### Authentication

```http
POST /api/auth/login
```

### Students

```http
GET    /api/students
GET    /api/students/{id}
POST   /api/students
PUT    /api/students/{id}
DELETE /api/students/{id}
```

### Dashboard

```http
GET /api/dashboard/stats
```

---

## 🌱 Git Workflow for Interns

### Step 1: Fork Repository

Fork this repository into your GitHub account.

### Step 2: Clone Repository

```bash
git clone https://github.com/your-username/student-management-system.git
```

### Step 3: Create Branch

```bash
git checkout -b feature/your-feature-name
```

Example:

```bash
git checkout -b feature/add-search-filter
```

### Step 4: Make Changes

Implement your feature.

### Step 5: Commit Changes

```bash
git add .
git commit -m "Added student search feature"
```

### Step 6: Push Changes

```bash
git push origin feature/add-search-filter
```

### Step 7: Raise Pull Request

Open GitHub and create a Pull Request to the `main` branch.

---

## 📸 Screenshots

Add your application screenshots inside the `screenshots/` folder:
