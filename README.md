# ServiceHub - Provider Service

## 📌 Overview

The **Provider Service** is a microservice of the ServiceHub Home Service Request System.

It is responsible for managing service provider-related information and operations.

Main responsibilities include:

- Managing service providers
- Managing provider information
- Managing provider availability
- Managing provider service details
- Supporting service request assignments

---

## 👨‍🎓 Student Information

| Information | Details |
|---|---|
| Student Name | Yashoda Gunawardhana |
| Student ID | 241711077 |
| Project | ServiceHub |
| Microservice | Provider Service |
| GCP Project ID | project-a6d8ea92-fb5d-4ed6-99d |

---

## 🛠️ Technology Stack

- Java 25
- Spring Boot
- Spring Cloud
- Spring Data
- MySQL
- Spring Cloud Config
- Eureka Client
- Spring Web
- Maven
- Lombok

---

## 🏗️ Architecture

```
Frontend
    |
    v
API Gateway :8080
    |
    v
Provider Service :8083
    |
    v
Database


Config Server :8888
        |
        v
Provider Service


Eureka Server :8761
        |
        v
Provider Service
```

---

## 🗄️ Database

The Provider Service manages service provider information using a relational database.

```
Provider Service
       |
       v
Spring Data
       |
       v
MySQL
```

---

## 🔎 Service Discovery

The Provider Service registers with Eureka Server.

```
Provider Service :8083
        |
        v
Eureka Server :8761
```

---

## ⚙️ Configuration

The service uses Spring Cloud Config for centralized configuration.

```
Config Server :8888
        |
        v
Provider Service
```

---

## 🔌 Service Information

| Property | Value |
|---|---|
| Service Name | provider-service |
| Port | 8083 |
| Database | MySQL |
| Database Type | Relational |
| API Gateway | 8080 |
| Eureka Server | 8761 |
| Config Server | 8888 |

---

## 🚀 Running the Service

**Windows**

```bash
.\mvnw.cmd spring-boot:run
```

### Build

```bash
.\mvnw.cmd clean package
```

### Run Tests

```bash
.\mvnw.cmd test
```

---

## 📁 Project Structure

```
provider-service/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   └── resources/
│   │
│   └── test/
│
├── .gitignore
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```

---

## 🔗 GitHub Repository

https://github.com/yashodha-gunawardana/provider-service

---

## 📌 Project Status

- Java 25: ✅
- Spring Boot: ✅
- MySQL: ✅
- Eureka Client: ✅
- Config Client: ✅
- GitHub Repository: ✅
- GCP Deployment: ⏳

---
