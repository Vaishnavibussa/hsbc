My portal

Banking Portal - API-Driven Financial Data Aggregator
A secure banking platform with real-time analytics and role-based dashboards

✅ Overview
This project is designed as part of the API-Driven Financial Data Aggregator problem statement. It provides:
✔ Banking Portal API (Spring Boot) for managing user accounts, authentication, transactions, and security
✔ Banking Portal UI (Angular) for seamless user experience
✔ Data Analytics Dashboard (React + Material UI + Recharts) for financial visualization

✨ Features
✅ Core Banking Features
User Registration & Authentication (JWT-based, role-based access)

PIN Management (Create & update secure PINs)

Cash Deposit & Withdrawal

Fund Transfer (between accounts)

Transaction History with pagination

Secure API endpoints with Spring Security

✅ Data Analytics Dashboard
Fraud vs Non-Fraud Transaction Analysis

Transactions by Category

Average Transaction Amount by Gender

Visualization using Material UI + Recharts

CSV Upload & Dynamic Chart Rendering

🛠 Tech Stack
Backend (API):

Java 21, Spring Boot 3, Spring Security, Hibernate, MySQL, JWT Authentication

Frontend (UI):

Angular, Bootstrap

Analytics Dashboard:

React, Material UI, Recharts, Papaparse (CSV Parsing)

Other Tools:

Maven, Postman (API Testing), Swagger (API Documentation)

📂 Project Structure
bash
Copy
Edit
banking_fin/
│
├── BankingPortal-API      # Spring Boot Backend
│   ├── src/main/java/com/webapp/bankingportal
│   ├── application.properties
│   └── pom.xml
│
├── BankingPortal-UI       # Angular Frontend
│   ├── src/app
│   └── angular.json
│
└── FraudDashboard         # React + Material UI Charts
    ├── src/App.js
    └── package.json


    📊 Charts Implemented
Pie Chart: Fraud vs Non-Fraud Transactions

Bar Chart: Transactions by Category

Line Chart: Average Transaction Amount over Steps

🔐 Authentication
JWT Authentication implemented in API

Role-based Access Control (Admin, Client, User)

Login via /auth/login

Get JWT token → Add Authorization: Bearer <token> in Postman for secure endpoints

📑 API Documentation
Swagger URL: http://localhost:8080/swagger-ui.html

Postman Collection: [Banking Portal.postman_collection.json](./BankingPortal-API/Banking Portal.postman_collection.json)

✅ ER Diagram
Entities: User, Account, Transaction

One-to-One: User ↔ Account

One-to-Many: Account ↔ Transactions

🎯 Expected Outcomes
✔ Secure banking operations
✔ Real-time analytics dashboard
✔ Configurable, scalable API-driven architecture

📸 Screenshots
(Add your dashboard, UI & Postman screenshots here)

💡 Future Enhancements
Email notifications on account login

Bank statements via email

JWT token storage in DB

Advanced fraud detection using ML models