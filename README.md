# Ride-booking-app

# 🚗 Geolocation-Based Ride Booking App (Spring Boot Microservices)

A scalable, real-time ride booking platform built using Spring Boot microservices, supporting live driver tracking, secure JWT authentication, real-time client updates, and async communication.

## 🧩 Architecture Overview

This project follows a distributed microservices architecture with 7+ independently deployable services:

| Service Name       | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| [Auth Service](https://github.com/Divs-Git/UberProject-AuthService)         | Handles user and driver authentication using JWT.                     |
| [Booking Service](https://github.com/Divs-Git/UberProject-BookingService)   | Manages ride creation, driver assignment, and ride status updates.   |
| [Location Service](https://github.com/Divs-Git/UberProject-LocationService) | Updates and fetches live driver location using Redis GEO.            |
| [Socket Service](https://github.com/Divs-Git/SocketServerSpringBoot)     | Handles real-time communication using STOMP WebSockets.              |
| [Review Service](https://github.com/Divs-Git/UberProject-ReviewService)     | Manages CRUD for ride reviews.                                       |
| [Entity Service](https://github.com/Divs-Git/UberProject-EntityService)     | Contains shared DTOs, entity models, and enums used across services. |
| [Eureka Service](https://github.com/Divs-Git/UberProject-ServiceDiscovery)     | Service discovery server for registering all microservices.          |

---

## 🛠️ Tech Stack

- **Spring Boot**, **Spring Data JPA**, **Spring Web**
- **Spring Security + JWT** for authentication
- **Redis** for geolocation tracking
- **Kafka** for async messaging between services
- **Retrofit** for internal API communication
- **Flyway** for DB versioning and migrations
- **STOMP over WebSocket** for real-time events
- **Eureka** for service discovery

---

## 📌 Features

- Real-time ride updates using WebSockets
- Efficient driver discovery using Redis GEO commands
- Scalable event-driven architecture using Kafka
- Clean layered architecture with proper DTOs and repositories
- Secure JWT-based authentication with role-based access control

---

