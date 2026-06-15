# Smart Library System


LibTrack is a modern full-stack library automation platform built to streamline book inventory, member records, and borrowing workflows using Spring Boot, React, and MySQL.

---

# 🚀 Overview

LibTrack enables librarians and administrators to efficiently manage:

- Book inventory
- Library members
- Book lending and return workflows

The system follows a layered backend architecture and exposes RESTful APIs consumed by a React-based user interface.

This project highlights how modern applications integrate:

- Client-side UI (React)
- Backend REST APIs (Spring Boot REST API)
- Persistent relational databases (MySQL)

---

# 📌 Project Status

This project is designed as a scalable full-stack library automation solution focused on managing books, members, and lending workflows.

It currently supports CRUD operations for:

- 📚 Books
- 👤 Members
- 🔖 Loans

The backend exposes REST endpoints which are consumed by the React frontend.

Interactive API documentation is also available through **Swagger/OpenAPI**.

---

# 📘 Key Learning Areas

• Building REST APIs using Spring Boot
• Implementing CRUD operations with Spring Data JPA
• Structuring a layered backend architecture (Controller → Service → Repository)
• Using DTOs to decouple API contracts from JPA entities
• Connecting a React frontend to backend APIs
• Building controlled forms with dynamic dropdowns in React
• Managing relational data using MySQL
• Documenting APIs using Swagger/OpenAPI

---

# 🛠️ Tech Stack

## Frontend

* React

## Backend

* Java
* Spring Boot
* Spring Data JPA
* REST APIs
* Swagger / OpenAPI

## Database

* MySQL

---

# ✨ Features

## 📚 Book Management

The system provides complete CRUD functionality for managing books.

Users can:

• Add new books to the library catalog  
• View all books  
• Update book information  
• Delete books from the system  

---

## 👤 Member Management

Library members can also be managed through the API.

Users can:

• Register new members
• View all members
• Update member information
• Delete members

---

## 🔖 Loan Management

Books can be checked out to members and tracked through the system.

Users can:

• Create a loan by selecting a book and a member
• View all active and past loans
• Update loan details including return date
• Delete a loan record

---

# 📡 API Documentation

The backend includes **Swagger/OpenAPI documentation**.

After starting the backend server, open:

```

[http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

```

or

```

[http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)

````

Swagger allows you to:

- View all API endpoints
- Test requests directly from the browser
- Inspect request and response models

---

# 🏗️ Project Architecture

The application is organized into **three modules**:

### `backend-data`
Contains **JPA entities and persistence logic**.

### `backend-api`
Spring Boot **REST API** exposing endpoints for books and members.

### `frontend-web`
React frontend that communicates with the backend API.

---

# ⚙️ How to Run the Project

## 1️⃣ Clone the repository

```bash
git clone https://github.com/hinduri-thanmai/smart-library-system.git
````

---

## 2️⃣ Setup MySQL

Create the database:

```sql
CREATE DATABASE libtrack_db;
```

Update database credentials in:

```
libraryms-app-rest/src/main/resources/application.properties
```

---

## 3️⃣ Start the Backend

```bash
cd libraryms-app-rest
mvn spring-boot:run
```

Backend runs at:

```
http://localhost:8080
```

---

## 4️⃣ Start the Frontend

```bash
cd libraryms-app-web
npm install
npm start
```

Frontend runs at:

```
http://localhost:3000
```
---
---

# Future Scope

• Role-based access for admins and members  
• Book reservation system  
• Fine calculation for overdue books  
• Email notifications for due dates  
• Analytics dashboard

---
