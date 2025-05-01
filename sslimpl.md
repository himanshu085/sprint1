
# SSL Implementation

## Author

| **Author** | **Created on** | **Version** | **Last updated by** | **Last Edited On** | **Level**          | **Reviewer**    |
|------------|----------------|-------------|---------------------|--------------------|--------------------|-----------------|
| Himanshu   | 2025-05-02     | 1.0         | Himanshu            | 2025-05-02         | Internal Reviewer  | Komal Jaiswal   |
| Himanshu   | 2025-05-02     |             |                     |                    | L0                 | Imran           |
| Himanshu   | 2025-05-02     |             |                     |                    | L1                 | Shashi          |
| Himanshu   | 2025-05-02     |             |                     |                    | L2                 | Mahesh Kumar    |


## Table of Content

- [Introduction](#introduction)
- [Pre-requisites](#pre-requisites)
- [Implementation Steps](#implementation-steps)
- [Conclusion](#conclusion)
- [Contact Information](#contact-information)
- [Reference](#reference)


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

```sh
sudo nano /etc/nginx/sites-available/default
```
### Now Adding this Content as given below:

```sh
server {
    listen 80;
    server_name cloudninjahp.publicvm.com;
    client_max_body_size 100M;

    index index.html index.php;
    root /var/www/html/cloudninjahp.publicvm.com/;

    access_log  /var/log/nginx/cloudninjahp.publicvm.com/access.log;
    error_log   /var/log/nginx/cloudninjahp.publicvm.com/error.log;
}
```
### Create web root dir
```sh
sudo mkdir -p /var/www/html/cloudninjahp.publicvm.com
```

### Place your HTML file
```sh
sudo nano /var/www/html/cloudninjahp.publicvm.com/index.html
```
### Now Paste the HTML code
```sh
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Welcome to CloudNinja</title>
  <style>
    body {
      background: linear-gradient(to right, #00c6ff, #0072ff);
      color: white;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      text-align: center;
      padding-top: 15%;
    }
    h1 {
      font-size: 3em;
      font-weight: bold;
      margin-bottom: 0.3em;
      text-shadow: 2px 2px 4px #000000;
    }
    p {
      font-size: 1.5em;
      font-weight: bold;
      text-shadow: 1px 1px 2px #000000;
    }
  </style>
</head>
<body>
  <h1>WELCOME TO CLOUDNINJA PAGE</h1>
  <p>Maintained by Himanshu Parashar</p>
</body>
</html>
```
### Create log directories
```sh
sudo mkdir -p /var/log/nginx/cloudninjahp.publicvm.com
```
### Reload Nginx
```sh
sudo systemctl reload nginx
```
![Screenshot from 2025-05-02 00-43-31-Photoroom](https://github.com/user-attachments/assets/d9ed25de-14c2-4656-b076-3b9c2e98851f)

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
