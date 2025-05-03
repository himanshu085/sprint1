# Fullstack Documentation

## Author

| **Author** | **Created on** | **Version** | **Last updated by** | **Last Edited On** | **Level**          | **Reviewer**    |
|------------|----------------|-------------|---------------------|--------------------|--------------------|-----------------|
| Himanshu   | 2025-05-02     | 1.0         | Himanshu            | 2025-05-02         | Internal Reviewer  | Komal Jaiswal   |
| Himanshu   | 2025-05-02     |             |                     |                    | L0                 | Imran           |
| Himanshu   | 2025-05-02     |             |                     |                    | L1                 | Shashi          |
| Himanshu   | 2025-05-02     |             |                     |                    | L2                 | Mahesh Kumar    |

## Table of Contents
1. [Introduction](#introduction)
2. [Overall Component Architecture Flow](#overall-component-architecture-flow)
   * [Frontend Flow](#frontend-flow)
   * [Backend Management](#backend-management)
      * [Employee API](#1-employee-api)
      * [Salary API](#2-salary-api)
      * [Attendance API](#3-attendance-api)
    * [Middleware](#middleware)
    * [Database Management](#database-management)
3. [User Flow](#user-flow)
5. [Conclusion](#conclusion)
6. [Contact Information](#contact-information)
7. [Refrences](#references)
## Introduction
Full Stack Development is the process of creating a complete web application that includes front-end, back-end, and database management. 
- **Front-End**: This is what users see and interact with on the website. It focuses on the look and feel, making sure the site is easy to use and looks good.
- **Back-End**: This is the behind-the-scenes part. It handles the server, the logic of the application, and ensures everything works correctly. It also manages security and data processing.
- **Middleware**: Acts as a bridge between the front-end and back-end, handling communication, data processing, and tasks like authentication, logging, and error handling for smooth interaction.
  
- **Database Management**: This part is about storing and organizing all the data the application needs. It makes sure data can be easily accessed and managed.
---
## Overall Component Architecture Flow
### Frontend Flow
Frontend Web is a REACTJS based application that is the primary user-interface for OT-Microservices stack.The app is designed for cross-platform fuctionality and requires only the presence of javascript runtime modules.The ReactJS based web framework facilitates complete web page based operations.
## Application-Flow
The frontend application have dependencies on other REST API of OT-Microservices.
<img width="1412" alt="Frontend" src="https://github.com/user-attachments/assets/f63157ad-c346-44d9-a906-e02503421a30" />
To run the application successfully, These things should be configured
For Refrence Links Below :-
* [Frontend POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/himanshu-SCRUM-96/ot_ms_understanding/application/frontend/setup/README.md)
* [Employee API](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-86/ot_ms_understanding/application/employee/documentation/README.md)
* [Attendance API](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Pravesh-SCRUM-4/OT%20MS%20Understanding/Applications/Attendance/Documentation/README.md)
* [Salary API](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Mohit-SCRUM-9/OT%20MS%20Understanding/Applications/Salary/Documentation%20/README.md)
---
## Backend Management
#### 1. Employee-API
The Employee REST API is a Go-based microservice that manages all employee-related transactions within the OT-Microservices stack. It is fully platform-independent, meaning it can run on any type of operating system or platform.
<img width="1424" alt="Employee" src="https://github.com/user-attachments/assets/5b874918-cdca-4860-81b7-f378d7e9d9da" />
Create this same as above.
Pre-Requisites
For running the application, we need following things configured:
For Refrence Links Below :-
* [Documentation](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-86/ot_ms_understanding/application/employee/documentation/README.md)
* [Employee POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Tharik_SCRUM-83/ot_ms_understanding/application/employee/setup/README.md) 
* [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-110/ot_ms_understanding/software/database/scylladb/setup/README.md)
* [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
---
#### 2. Salary API
The Salary API is a Java-based microservice that handles all salary-related transactions and records within the OT-Microservices stack. It is platform-independent, meaning it can run on various operating systems. However, to run this application, a Java Runtime Environment (JRE) is required.
<img width="1424" alt="Salary" src="https://github.com/user-attachments/assets/df213ffb-2d1b-4ae7-85b0-963a3a151a55" />
We only need maven as build tool, but for running the application following things are required
For Refrence Link are below :-
* [Documentation](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Mohit-SCRUM-9/OT%20MS%20Understanding/Applications/Salary/Documentation%20/README.md)
* [Salary POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aniruddh_SCRUM-93/ot_ms_understanding/application/salary/setup/README.md)
* [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aditya_SCRUM-110/ot_ms_understanding/software/database/scylladb/setup/README.md)
* [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
* [Maven](https://github.com/Cloud-NInja-snaatak/Documentation/blob/shubham_scrum29/commonstack/applications/java/pom/sop.md)
---
#### 3. Attendance API
The Attendance REST API is a Python-based microservice that manages all attendance-related transactions within the OT-Microservices stack. This application is cross-platform, meaning it can run on different operating systems. The only requirement to run it is the Python runtime environment.
<img width="1412" alt="Attendance" src="https://github.com/user-attachments/assets/d5c86c62-9139-4a82-97ec-6efbd653e643" />
To run the application successfully, we need these things configured
PostgreSQL as a primary database for storing all the attendance records
Redis as cache management middleware for storing all API response
Below Have Refrence Links in detail :-
* [Documentation](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Pravesh-SCRUM-4/OT%20MS%20Understanding/Applications/Attendance/Documentation/README.md) 
* [Attendance POC](https://github.com/Cloud-NInja-snaatak/Documentation/blob/SHREY-SCRUM-70/ot_ms_understanding/application/attendance/setup/README.md) 
* [PostgreSQL](https://github.com/snaatak-Zero-Downtime-Crew/Documentation/blob/Pooja-SCRUM-14/OT%20MS%20Understanding/Database/PostgreSQL/POC/Readme.md)
* [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_SCRUM-106/ot_ms_understanding/software/middleware/redis/setup/README.md)
* [Poetry](https://github.com/Cloud-NInja-snaatak/Documentation/blob/rajeev_scrum18/commonstack/applications/python/poetry/sop.md)
* [Liquibase](https://github.com/Cloud-NInja-snaatak/Documentation/blob/SHREY-SCRUM-116/db_change_management/db_release_management/poc_liquibase/README.md)
---
### Middleware
Middleware acts as a bridge between the frontend and backend, enabling communication and optimizing performance. In the OT-Microservices, Redis is used as a caching middleware to store frequently accessed data, such as employee, salary and attendance records, reducing database load and improving response times.
For Refrence Links Below :-
* [Redis](https://github.com/Cloud-NInja-snaatak/Documentation/tree/SHREY-SCRUM-107/ot_ms_understanding/software/middleware/redis/documentation)
---
### Database Management
Database management is responsible for storing, accessing, and managing data for an application. It involves tasks such as creating databases, maintaining their performance, and optimizing them to ensure efficient data handling.
For Refrence Links Below :-
* [ScyllaDB](https://github.com/Cloud-NInja-snaatak/Documentation/blob/aniruddh_SCRUM-111/ot_ms_understanding/software/database/scylladb/documentation/README.md)
    *  ScyllaDB is the main NoSQL database in the OT-Microservices stack, used to store **`employee`** and **`salary`** data. It is highly scalable and designed for fast performance in large applications.
  
* [PostgreSQL](https://github.com/Cloud-NInja-snaatak/Documentation/blob/Tharik_SCRUM-109/ot_ms_understanding/software/database/postgressql/documentation/README.md)
  
   *  PostgreSQL is the relational database in the OT-Microservices stack, used for storing **`attendance`** records. It is reliable, supports complex queries, and ensures data consistency.
---
### User Flow
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

## Contact Information
| Name              | Email Address                                   |
|-------------------|--------------------------------------------------|
| Himanshu Parashar | himanshu.parashar.snaatak@mygurukulam.co         |

## References
| **Link**                                                                                                                     | **Description**                                    |
|-----------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| [API Repo Link](https://github.com/OT-MICROSERVICES) | APIs Documentation    |
