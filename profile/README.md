# 🛫 Airplane Booking System — Microservices Architecture

This organization contains the backend microservices for an **Airplane Booking System**, built using a microservices architecture. The system is divided into two independent services — one for managing flight-related data and the other for handling bookings and payments.

Each microservice is developed using **Node.js**, **Express.js**, **PostgreSQL**, and **Prisma ORM**, following clean code practices and RESTful API standards.

---

## 🧩 Microservices Overview

### 1. ✈️ [Flights-Service](https://github.com/<your-org>/Flights-Service)

Handles all data related to:

- Flights
- Airplanes
- Cities
- Airports

**Features:**

- Full CRUD APIs for flight-related entities
- Prisma ORM for database management
- Search & seat management
- Easily extendable and modular

---

### 2. 🎟️ [Flight-Booking-Service](https://github.com/<your-org>/Flight-Booking-Service)

Responsible for:

- Booking flights
- Simulating payments
- Enforcing a 5-minute payment rule
- Auto-canceling unpaid bookings with cron jobs

**Features:**

- Transactional consistency using row-level locks
- Background cron job for cleaning stale bookings
- Payment API logic and booking lifecycle handling

---

## ⚙️ Technologies Used

- Node.js & Express.js
- PostgreSQL
- Prisma ORM
- JavaScript
- Cron Jobs

---

## 🛠️ How to Run the System Locally

1. **Start the Flights-Service**
2. **Start the Flight-Booking-Service** (ensure it connects to Flights-Service via `FLIGHT_SERVICE` env variable)
3. Seed databases and test endpoints using Postman or any API testing tool.

> 💡 Each microservice has its own detailed README with setup instructions and API documentation.

---

## 📂 Architecture Style

This project follows a **microservices architecture**, which offers:

- Clear separation of concerns
- Easier maintenance and scaling
- Independent deployment and development


---
