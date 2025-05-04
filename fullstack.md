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
- [OT-Microservices System Architecture Flow](#ot-microservices-system-architecture-flow)
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

**Full Stack Development** refers to building a complete web application that encompasses the front end, back end, and database management.

- **Front End**: This is the user-facing part of the application — everything users see and interact with. It focuses on visual design, user experience, and ensuring the interface is intuitive and responsive.

- **Back End**: This is the server-side component that powers the application behind the scenes. It manages application logic, processes data, handles security, and ensures seamless functionality.

- **Database Management**: This involves storing, organizing, and managing the application’s data. It ensures data is efficiently stored, easily accessible, and reliably maintained.

---

## OT-Microservices System Architecture Flow

### Frontend Flow

The frontend application is a **ReactJS-based** web interface that serves as the primary user interface for the OT-Microservices stack. It is designed for **cross-platform functionality** and requires only a JavaScript runtime environment to operate. The ReactJS framework enables a fully interactive, single-page application experience, supporting seamless and efficient user interactions across devices.

The frontend application has dependencies on other REST APIs of OT-Microservices.

![Screenshot from 2025-05-03 20-07-16](https://github.com/user-attachments/assets/59ea43b1-adef-4001-8921-08a02779b1d6)


To run the application successfully, these things should be configured:

- [Frontend POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/himanshu-SCRUM-96/ot_ms_understanding/application/frontend/setup/README.md)
- [Employee DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-86/ot_ms_understanding/application/employee/documentation/README.md)
- [Attendance DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Shubham_SCRUM-72/ot_ms_understanding/application/attendance/documentation/README.md)
- [Salary DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/anitha-SCRUM-95/ot_ms_understanding/application/salary/documentation/README.md)

---

## Backend Management

### Employee API

The Employee REST API is a Go-based microservice responsible for managing employee-related workflows within the OT-Microservices stack. It is fully platform-independent, capable of operating across various operating systems and platforms.


![Screenshot from 2025-05-03 20-05-05](https://github.com/user-attachments/assets/6811a34e-cd66-4fd6-9e06-c996d02b56c3


Pre-Requisites for running the application:

- [Employee Documentation](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-86/ot_ms_understanding/application/employee/documentation/README.md)
- [Employee POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Tharik_SCRUM-83/ot_ms_understanding/application/employee/setup/README.md)
- [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-110/ot_ms_understanding/software/database/scylladb/setup/README.md)
- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)

---

### Salary API

The Salary API is a Java-based microservice responsible for managing salary-related transactions and data within the OT-Microservices stack. It offers platform independence, allowing it to operate across various operating systems, though a Java Runtime Environment (JRE) is necessary for its execution.


![Screenshot from 2025-05-03 20-06-04](https://github.com/user-attachments/assets/cda1a896-da57-4e4c-8666-598816d0c51f)


Maven is the only required build tool, though the following components are essential for running the application:


- [Salary Documentation](https://github.com/Cloud-NInja-snaatak/Documentation/blob/anitha-SCRUM-95/ot_ms_understanding/application/salary/documentation/README.md)
- [Salary POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aniruddh_SCRUM-93/ot_ms_understanding/application/salary/setup/README.md)
- [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-110/ot_ms_understanding/software/database/scylladb/setup/README.md)
- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
- [Maven](https://github.com/Cloud-NInja-snaatak/Documentation/blob/shubham_scrum29/commonstack/applications/java/pom/sop.md)

---

### Attendance API

Built using Python, the Attendance REST API handles all attendance-related processes within the OT-Microservices stack. This cross-platform application only requires a Python runtime environment to function.


![Screenshot from 2025-05-03 20-05-35](https://github.com/user-attachments/assets/98957e35-d7cc-48ab-bf30-1a48a56c381c)


Successful execution of the application requires the following configurations:


- [Atttendance Documentation](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Shubham_SCRUM-72/ot_ms_understanding/application/attendance/documentation/README.md)
- [Attendance POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/SHREY-SCRUM-70/ot_ms_understanding/application/attendance/setup/README.md)
- [PostgreSQL](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Shubham_SCRUM-108/ot_ms_understanding/software/database/postgressql/setup/README.md)
- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
- [Poetry](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_scrum18/commonstack/applications/python/poetry/sop.md)
- [Liquibase](https://github.com/Cloud-NInja-snaatak/Documentation/blob/SHREY-SCRUM-116/db_change_management/db_release_management/poc_liquibase/README.md)

---

### Middleware

Middleware acts as a connector between the frontend and backend, facilitating efficient communication and optimizing performance. In OT-Microservices, Redis is used as a caching layer to hold frequently accessed data, like employee, salary, and attendance records, thereby reducing the strain on the database and enhancing response speed.


- [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/tree/SHREY-SCRUM-107/ot_ms_understanding/software/middleware/redis/documentation)

---

### Database Management

Database management focuses on storing, accessing, and organizing application data. It includes tasks such as setting up databases, ensuring optimal performance, and maintaining them for reliable and efficient data handling.

- [ScyllaDB DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aniruddh_SCRUM-111/ot_ms_understanding/software/database/scylladb/documentation/README.md)  

   ScyllaDB serves as the primary NoSQL database within the OT-Microservices stack, storing **`employee`** and **`salary`** data. It is engineered for high scalability and delivers fast performance, making it ideal for large-scale applications.

- [PostgreSQL DOC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Tharik_SCRUM-109/ot_ms_understanding/software/database/postgressql/documentation/README.md)  

  PostgreSQL serves as the relational database within the OT-Microservices stack, dedicated to storing **`attendance`** records. It offers robust reliability, supports complex queries, and ensures strong data consistency.

---

## User Flow

| **User Registration Flow** |                
|----------------------------|
| 1. The user fills out and submits the registration form. |     
| 2. The frontend validates the provided input. |                                     
| 3. The validated request is forwarded to the backend. |                       
| 4. The backend processes the registration and stores the user data in the database. |        
| 5. A success response is returned to the frontend. |                                      
---

| **User Login Flow** |                                                  
|---------------------|                                      
| 1. The user submits the login form with credentials. |                                       
| 2. The frontend validates the input data. |                                           
| 3. The request is forwarded to the backend. |                                     
| 4. The backend authenticates the user credentials. |                                    
| 5. A response containing an authentication token is returned to the frontend. |            
---

| **Data Processing Flow** |                                                                                        
|---------------------------|
| 1. Data is submitted from the frontend interface. |                                                               
| 2. The backend processes the incoming data. |                                                                         
| 3. The data is validated and transformed as required. |                                                                
| 4. The processed data is stored in the database. |                                                           
| 5. A confirmation response is sent back to the frontend. |  
---


## Conclusion

This document provides a comprehensive overview of full-stack development within the **OT-Microservices** project. It outlines the integration of the **frontend**, **middleware**, and **backend** components, and highlights key practices for building robust and maintainable applications.


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
