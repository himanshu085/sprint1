
# SSL Implementation

## Author

| **Author** | **Created on** | **Version** | **Last updated by** | **Last Edited On** | **Level**          | **Reviewer**    |
|------------|----------------|-------------|---------------------|--------------------|--------------------|-----------------|
| Himanshu   | 2025-05-02     | 1.0         | Himanshu            | 2025-05-02         | Internal Reviewer  | Komal Jaiswal   |
| Himanshu   | 2025-05-02     |             |                     |                    | L0                 | Imran           |
| Himanshu   | 2025-05-02     |             |                     |                    | L1                 | Shashi          |
| Himanshu   | 2025-05-02     |             |                     |                    | L2                 | Mahesh Kumar    |


## Table of Content

1. [Introduction](#introduction)
2. [Pre-requisites](#pre-requisites)
3. [Implementation Steps](#implementation-steps)
4. [Conclusion](#conclusion)
5. [Contact Information](#contact-information)
6. [Reference](#reference)

## Introduction

This document explains the implementation of an SSL certificate on the domain as per POC. Here we are using **Certbot**, an open-source SSL certification authority, and the server we are using is **Nginx**.

## Pre-requisites

- **Domain Name**: Domain DNS configured to point to the server (A/AAAA records).
- **Web server**: Install **Nginx** server on your VM.

## Implementation Steps

### 1. Install Certbot

Update system packages and install Certbot.
![Screenshot from 2025-05-02 00-42-45](https://github.com/user-attachments/assets/24fbc483-580a-4ecf-ac12-a89909db3240)


### 2. Verify Server Configuration

Check Nginx to ensure your domain is being served correctly.

### 3. Obtain SSL Certificate

Run the Certbot command for your domain:
```bash
sudo certbot --nginx -d cloudninjahp.publicvm.com
```
![Screenshot from 2025-05-02 01-33-38](https://github.com/user-attachments/assets/51643a66-ecf5-4571-959d-09fa0e803acc)

### 4. Update Web Server Configuration

Certbot will automatically update the server configuration. Verify the changes by looking for the `listen 443 ssl` block added by Certbot.
```sh
sudo vi /etc/nginx/sites-available/default
```
![Screenshot from 2025-05-02 01-53-26](https://github.com/user-attachments/assets/8e8005f6-2472-4e39-8631-8f6445972e3f)


### 5. Restart Web Server

Reload the server to apply the changes:
```bash
sudo systemctl reload nginx
```
![Screenshot from 2025-05-02 01-59-20](https://github.com/user-attachments/assets/96a5aa42-6ef5-436c-b874-53a65dd2e598)

### 6. Validate SSL

Open `https://cloudninjahp.publicvm.com/` in a browser and ensure it shows a secure lock icon.
![Screenshot from 2025-05-02 01-26-42](https://github.com/user-attachments/assets/9b86dc98-54d5-42d9-9737-e4ea7ca68560)


## Conclusion

The domain now uses SSL encryption provided by **Let’s Encrypt**, improving security and user trust. The process is free and includes automated renewal for uninterrupted protection.

##  **Contact Information**

| Name              | Email Address                                   |
|-------------------|--------------------------------------------------|
| Himanshu Parashar | himanshu.parashar.snaatak@mygurukulam.co         |

## Reference

| **Reference Name**  | **Description**                            | **Link**                |
|---------------------|--------------------------------------------|-------------------------|
| SSL POC             | POC on how you can set up SSL for your Domain | SSL POC                 |
| SSL Documentation   | Detailed documentation on SSL              | SSL Documentation       |
