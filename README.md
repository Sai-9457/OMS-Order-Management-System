# Order Management System (OMS) – Backend

A REST-based backend application built using **Java** and **Spring Boot** to manage orders and their lifecycle.  
This project follows a clean layered architecture and demonstrates real-world backend development practices.

---

## 🚀 Tech Stack
- Java
- Spring Boot
- Spring Data JPA
- MySQL
- Hibernate
- Maven

---

## 🧱 Architecture
The application follows **Layered Architecture**:

- **Controller Layer** – Handles HTTP requests and responses
- **Service Layer** – Contains business logic
- **Repository Layer** – Handles database operations using JPA
- **Model Layer** – Entity and enum definitions

---

## 📌 Features
- Create new orders
- Fetch all orders
- Update order lifecycle status:
    - CREATED
    - PACKED
    - SHIPPED
    - DELIVERED
- RESTful API design
- MySQL database integration
- Hibernate ORM for persistence

---

## 📂 Project Structure
```
src/main/java/com/example/OMS
├── controller
│ └── OrderController.java
├── service
│ └── OrderService.java
├── repository
│ └── OrderRepository.java
├── model
│ ├── Order.java
│ └── OrderStatus.java
└── OrderManagementSystemApplication.java
```

---

## How to Run

Run the application using the following command from the project root directory:

```bash
mvn spring-boot:run
```
## Application runs on: http://localhost:8080

## API Endpoints

- **POST** `/api/orders` – Create a new order  
- **GET** `/api/orders` – Fetch all orders  
- **PUT** `/api/orders/{id}/status` – Update order lifecycle status  


