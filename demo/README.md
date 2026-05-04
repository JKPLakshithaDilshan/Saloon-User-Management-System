# Saloon User Management System

A robust and professional user management module designed for a Salon Management System. This project is built using **Spring Boot 3** and **Java 21**, focusing on clean code practices and core Object-Oriented Programming (OOP) principles.

## 🚀 Features

- **User Registration:** Secure signup with real-time validation for names, phone numbers, and strong passwords.
- **User Authentication:** Secure login system with credential verification.
- **Profile Management:** Users can view and update their profiles, including contact details and passwords.
- **File-Based Persistence:** Implements a custom CSV-based storage system for user data, eliminating the need for a complex database setup for lightweight applications.
- **Responsive UI:** A beautiful, responsive frontend built with Thymeleaf and Bootstrap, featuring Salon-specific pages (Services, Gallery, Blog).
- **OOP Excellence:** Demonstrates key concepts such as Encapsulation, Abstraction, and the Singleton Pattern.

## 🛠️ Technology Stack

- **Backend:** Java 21, Spring Boot 3.5.13
- **Frontend:** Thymeleaf Template Engine, HTML5, SCSS, Bootstrap 4
- **Persistence:** CSV File Storage (`data/users.txt`)
- **Build Tool:** Maven
- **Utilities:** Lombok, Java NIO

## 📂 Project Structure

```text
src/main/java/com/example/demo/
├── controller/      # Web controllers for routing and authentication
├── model/           # User data model with validation logic
├── repository/      # File-based data access layer (Singleton)
├── service/         # Business logic layer
└── util/            # Helper classes for file handling
```

## ⚙️ Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/Saloon-User-Management-System.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd demo
   ```

3. **Build the project:**
   ```bash
   ./mvnw clean install
   ```

4. **Run the application:**
   ```bash
   ./mvnw spring-boot:run
   ```

5. **Access the application:**
   Open your browser and go to `http://localhost:8080`

## 📖 Architecture & OOP Concepts

This project is designed as an educational and practical example of OOP:
- **Encapsulation:** User data is protected with private fields and public getters/setters with validation.
- **Abstraction:** The persistence logic is abstracted away into the `UserRepository`, allowing the rest of the app to interact with data without knowing it's a CSV file.
- **Singleton Pattern:** The `UserRepository` ensures only one instance manages the data file.
- **Information Hiding:** Critical logic like password strength verification is kept private within the model.

---
Developed by [Lakshitha Dilshan](https://github.com/your-username)
