# EC2 + Aurora Web App Project

Welcome to my cloud computing project where I built a fully functional web application running on an EC2 instance, connected to an Amazon Aurora MySQL database. This project demonstrates a classic architecture pattern used in real-world applications — connecting a web frontend to a relational backend database.

---

## 🛠 Technologies Used  

<p align="left">
  <img src="https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="Amazon EC2">
  <img src="https://img.shields.io/badge/Amazon%20Aurora-527FFF?style=for-the-badge&logo=amazonaws&logoColor=white" alt="Amazon Aurora">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/Apache%20HTTP%20Server-D22128?style=for-the-badge&logo=apache&logoColor=white" alt="Apache HTTP Server">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/SSH-4D4D4D?style=for-the-badge&logo=gnubash&logoColor=white" alt="SSH">
  <img src="https://img.shields.io/badge/AWS%20CLI-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS CLI">
</p>

---

## Architecture

This project follows a classic 2-tier architecture where the frontend (web app) is hosted on an EC2 instance and connects to a backend Aurora MySQL database.

<p>
  <img src="https://github.com/user-attachments/assets/51819cd8-f3d8-4443-8855-2cc2f74b6e6a" alt="Architecture Diagram" width="700">
</p>

**1. Frontend/Web Tier**  
- Apache + PHP running on EC2  
- Sample form to submit and display user data  

**2. Backend/Database Tier**  
- Amazon Aurora MySQL-compatible DB  
- Connected using PHP `MySQLi` extension  

---

## What I Did

- Launched an **EC2 instance** to host a web server  
- Created an **Aurora MySQL Database Cluster**  
- Connected EC2 to Aurora using PHP + MySQLi  
- Built a **PHP web app** that:
  - Accepts `name` and `address` input
  - Displays saved entries from the database
- Verified DB updates via **MySQL CLI**
- Used **IAM best practices** and secure key pairs
- **Cleaned up** AWS resources after the project

---

## Web App & Database Demo

A visual walkthrough of the full flow: from submitting data on the web app to verifying it in the database via CLI.

---

**1. Initial state of the PHP web app (hosted on EC2):**

<p>
  <img src="https://github.com/user-attachments/assets/bfd41551-20d5-43c7-8d5d-e40c9eec9475" width="700">
</p>

---

**2. After submitting data, the app displays it live (fetched from Aurora):**

<p>
  <img src="https://github.com/user-attachments/assets/94b810f6-19ee-49e9-9f7c-e82105c655d1" width="700">
</p>

---

**3. Verified the `EMPLOYEES` table structure using MySQL CLI:**

<p>
  <img src="https://github.com/user-attachments/assets/c83bb1b8-4cca-4d31-a118-95c9dbfa4bf2" width="700">
</p>

---

**4. Queried the table to confirm the submitted data exists:**

<p>
  <img src="https://github.com/user-attachments/assets/b3f93b49-4db3-4c6f-a50c-b9ef79c12fb5" width="700">
</p>
