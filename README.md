# 🎓 Student Result Management System

A full stack web application built using **Spring Boot** backend 
and a static **HTML/CSS/JavaScript** frontend that allows users 
to add and view student academic results with automatic grade 
calculation.

---

## 📌 Features

- Add student name, subject, and marks via a simple form
- Automatic grade calculation based on marks entered
- Fetches and displays all records dynamically in a result table
- REST API backend with Cross-Origin support
- No external database setup required — uses H2 in-memory database
- Clean and responsive UI

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend Framework | Spring Boot 4.0.4 |
| REST Controller | Spring Web MVC |
| ORM / Data Layer | Spring Data JPA |
| Database | H2 In-Memory Database |
| Frontend | HTML, CSS, JavaScript (Fetch API) |
| Build Tool | Apache Maven |
| Language | Java 17 |

---

## 📂 Project Structure

student-result/
├── src/
│   └── main/
│       ├── java/com/college/student_result/
│       │   ├── StudentResultApplication.java
│       │   ├── Student.java           # Entity class
│       │   ├── StudentRepository.java # JPA Repository
│       │   └── StudentController.java # REST Controller
│       └── resources/
│           ├── static/
│           │   └── index.html         # Frontend UI
│           └── application.properties
├── pom.xml
└── README.md


---

## 🔗 REST API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | /api/students | Fetch all student results |
| POST | /api/students | Add a new student result |

---

## ⚙️ Prerequisites

- Java 17 or above
- VS Code with Extension Pack for Java
- Spring Boot Extension Pack (VS Code)
- Any modern web browser 

---

## 🚀 How to Run

**Step 1 — Clone the repository**
```bash
git clone https://github.com/your-username/student-result.git
```

**Step 2 — Navigate into the project folder**
```bash
cd student-result
```

**Step 3 — Run the application**

On Windows:
```bash
.\mvnw.cmd spring-boot:run
```

On Mac/Linux:
```bash
./mvnw spring-boot:run
```

**Step 4 — Open in browser**
http://localhost:8080

---

## 🗄️ H2 Database Console
http://localhost:8080/h2-console

| Field | Value |
|---|---|
| JDBC URL | jdbc:h2:mem:testdb |
| Username | sa |
| Password | *(leave blank)* |

---

## 📊 Grade Calculation Logic

| Marks Range | Grade |
|---|---|
| 90 – 100 | O (Outstanding) |
| 80 – 89 | A (Excellent) |
| 70 – 79 | B (Very Good) |
| 60 – 69 | C (Good) |
| 50 – 59 | D (Average) |
| 40 – 49 | P (Pass) |
| Below 40 | F (Fail) |


## Developed for 

Java Full Stack Developer Virtual Internship — EduSkills (AICTE)
January 2026 – March 2026

---

## 📄 License

This project is developed for academic and internship purposes.