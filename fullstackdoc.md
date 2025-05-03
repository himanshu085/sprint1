<p align="center">
  <img src="https://github.com/user-attachments/assets/082af180-a168-4bfc-9f2f-5113d03382da" alt="Screenshot from 2025-05-03 20-01-32" width="400"/>
</p>

# Fullstack Documentation

## Author

| **Author** | **Created on** | **Version** | **Last updated by** | **Last Edited On** | **Level**          | **Reviewer**    |
|------------|----------------|-------------|---------------------|--------------------|--------------------|-----------------|
| Himanshu   | 2025-05-02     | 1.0         | Himanshu            | 2025-05-02         | Internal Reviewer  | Komal Jaiswal   |
| Himanshu   | 2025-05-02     |             |                     |                    | L0                 | Imran           |
| Himanshu   | 2025-05-02     |             |                     |                    | L1                 | Shashi          |
| Himanshu   | 2025-05-02     |             |                     |                    | L2                 | Mahesh Kumar    |

## Table of Contents

- [Introduction](#introduction)
- [Overall Component Architecture Flow](#overall-component-architecture-flow)
  - [Frontend Flow](#frontend-flow)
  - [Backend Management](#backend-management)
    - [Employee API](#employee-api)
    - [Salary API](#salary-api)
    - [Attendance API](#attendance-api)
  - [Middleware](#middleware)
  - [Database Management](#database-management)
- [User Flow](#user-flow)
- [Conclusion](#conclusion)
- [Contact Information](#contact-information)
- [References](#references)

---

## Introduction

Full Stack Development is the process of creating a complete web application that includes front-end, back-end, and database management.

- **Front-End**: This is what users see and interact with on the website. It focuses on the look and feel, making sure the site is easy to use and looks good.
- **Back-End**: This is the behind-the-scenes part. It handles the server, the logic of the application, and ensures everything works correctly. It also manages security and data processing.
- **Middleware**: Acts as a bridge between the front-end and back-end, handling communication, data processing, and tasks like authentication, logging, and error handling for smooth interaction.
- **Database Management**: This part is about storing and organizing all the data the application needs. It makes sure data can be easily accessed and managed.

---

## Overall Component Architecture Flow

### Frontend Flow

Frontend Web is a REACTJS based application that is the primary user-interface for OT-Microservices stack. The app is designed for cross-platform functionality and requires only the presence of javascript runtime modules. The ReactJS based web framework facilitates complete web page based operations.

The frontend application has dependencies on other REST APIs of OT-Microservices.

![Screenshot from 2025-05-03 20-07-16](https://github.com/user-attachments/assets/23f802a1-0516-4c0c-866b-818c8a839eaa)


To run the application successfully, these things should be configured:

- [Frontend POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/himanshu-SCRUM-96/ot_ms_understanding/application/frontend/setup/README.md)
- [Employee DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-86/ot_ms_understanding/application/employee/documentation/README.md)
- [Attendance DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Shubham_SCRUM-72/ot_ms_understanding/application/attendance/documentation/README.md)
- [Salary DOC](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Mohit-SCRUM-9/OT%20MS%20Understanding/Applications/Salary/Documentation%20/README.md)

---

## Backend Management

### Employee API

The Employee REST API is a Go-based microservice that manages all employee-related transactions within the OT-Microservices stack. It is fully platform-independent, meaning it can run on any type of operating system or platform.

![Screenshot from 2025-05-03 20-05-05](https://github.com/user-attachments/assets/6811a34e-cd66-4fd6-9e06-c996d02b56c3


Pre-Requisites for running the application:

- [Employee Documentation](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-86/ot_ms_understanding/application/employee/documentation/README.md)
- [Employee POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Tharik_SCRUM-83/ot_ms_understanding/application/employee/setup/README.md)
- [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-110/ot_ms_understanding/software/database/scylladb/setup/README.md)
- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)

---

### Salary API

The Salary API is a Java-based microservice that handles all salary-related transactions and records within the OT-Microservices stack. It is platform-independent, meaning it can run on various operating systems. However, to run this application, a Java Runtime Environment (JRE) is required.

![Screenshot from 2025-05-03 20-06-04](https://github.com/user-attachments/assets/cda1a896-da57-4e4c-8666-598816d0c51f)


We only need Maven as build tool, but for running the application following things are required:

- [Salary Documentation](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Mohit-SCRUM-9/OT%20MS%20Understanding/Applications/Salary/Documentation%20/README.md)
- [Salary POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aniruddh_SCRUM-93/ot_ms_understanding/application/salary/setup/README.md)
- [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-110/ot_ms_understanding/software/database/scylladb/setup/README.md)
- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
- [Maven](https://github.com/Cloud-NInja-snaatak/Documentation/blob/shubham_scrum29/commonstack/applications/java/pom/sop.md)

---

### Attendance API

The Attendance REST API is a Python-based microservice that manages all attendance-related transactions within the OT-Microservices stack. This application is cross-platform, meaning it can run on different operating systems. The only requirement to run it is the Python runtime environment.

![Screenshot from 2025-05-03 20-05-35](https://github.com/user-attachments/assets/98957e35-d7cc-48ab-bf30-1a48a56c381c)


To run the application successfully, we need these things configured:

- [Atttendance Documentation](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Shubham_SCRUM-72/ot_ms_understanding/application/attendance/documentation/README.md)
- [Attendance POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/SHREY-SCRUM-70/ot_ms_understanding/application/attendance/setup/README.md)
- [PostgreSQL](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Shubham_SCRUM-108/ot_ms_understanding/software/database/postgressql/setup/README.md)
- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
- [Poetry](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_scrum18/commonstack/applications/python/poetry/sop.md)
- [Liquibase](https://github.com/Cloud-NInja-snaatak/Documentation/blob/SHREY-SCRUM-116/db_change_management/db_release_management/poc_liquibase/README.md)

---

### Middleware

Middleware acts as a bridge between the frontend and backend, enabling communication and optimizing performance. In the OT-Microservices, Redis is used as a caching middleware to store frequently accessed data, such as employee, salary and attendance records, reducing database load and improving response times.

- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/tree/SHREY-SCRUM-107/ot_ms_understanding/software/middleware/redis/documentation)

---

### Database Management

Database management is responsible for storing, accessing, and managing data for an application. It involves tasks such as creating databases, maintaining their performance, and optimizing them to ensure efficient data handling.

- [ScyllaDB DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aniruddh_SCRUM-111/ot_ms_understanding/software/database/scylladb/documentation/README.md)  
  ScyllaDB is the main NoSQL database in the OT-Microservices stack, used to store **`employee`** and **`salary`** data. It is highly scalable and designed for fast performance in large applications.
- [PostgreSQL DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Tharik_SCRUM-109/ot_ms_understanding/software/database/postgressql/documentation/README.md)  
  PostgreSQL is the relational database in the OT-Microservices stack, used for storing **`attendance`** records. It is reliable, supports complex queries, and ensures data consistency.

---

## User Flow

| **User Registration Flow** |                
|---------------|
| 1. User submits the registration form. |     
| 2. Frontend validates the input. |                                     
| 3. The request is sent to the backend. |                       
| 4. The backend processes the registration and stores the data in the database. |        
| 5. A response is sent back to the frontend. |                                      
---
| **User Login Flow** |                                                  
|---------------------|                                      
| 1. User submits the login form. |                                       
| 2. Frontend validates the input. |                                           
| 3. The request is sent to the backend. |                                     
| 4. The backend authenticates the user. |                                    
| 5. A response is sent back to the frontend with a token. |            
---
| **Data Processing Flow** |                                                                                        
|---------------------------|
| 1. Data is submitted from the frontend. |                                                               
| 2. The backend processes the data. |                                                                         
| 3. Data is validated and transformed. |                                                                
| 4. Processed data is stored in the database. |                                                           
| 5. Confirmation is sent back to the frontend. |  
---

## Conclusion

This document gives a clear overview of full-stack development for the OT-MICROSERVICES project. It explains how the front end middleware and back end work together and shares important practices for building strong and easy-to-maintain applications.

---

## Contact Information

| Name              | Email Address                                   |
|-------------------|-------------------------------------------------|
| Himanshu Parashar | himanshu.parashar.snaatak@mygurukulam.co        |

---

## References

| **Link** | **Description** |
|----------|-----------------|
| [API Repo Link](https://github.com/OT-MICROSERVICES) | APIs Documentation |
