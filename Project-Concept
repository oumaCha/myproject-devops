# Project Concept: Student Management System Deployment

## Overview
The project aims to implement the full software lifecycle for deploying and automating the **Student Management System** application, using Infrastructure-as-Code (IaC) practices and cloud-based infrastructure. The system will be hosted on **AWS** and containerized using **Docker**, with all infrastructure and services provisioned and managed through **Terraform**. CI/CD pipelines will be implemented using **GitHub Actions**.
The Application **Student Management System** is inspired from an open source project here is the link: https://github.com/BobsProgrammingAcademy/student-management-system
However, the Application is already created in my Local Machine.
## Technology Stack
- **Version Control System (VCS)**: **GitHub** (for source code management)
- **Infrastructure-as-Code**: **Terraform** (for provisioning and managing infrastructure)
- **Application**: **Student Management System** (using **SQLite** as the initial database, with the possibility of scaling to **PostgreSQL** or **MySQL**)
- **CI/CD**: **GitHub Actions** (for automating builds, tests, and deployments)
- **Containerization**: **Docker** (to containerize the application)
- **Reverse Proxy**: **Nginx** (for routing traffic and handling SSL/TLS termination)
- **HTTPS Security**: **Let’s Encrypt** (for securing communication via SSL/TLS)

---

## Life Cycle of the Application

### 1. **Development and Version Control**
The development of the **Student Management System** will be tracked using **GitHub**. The application will be built with **SQLite** for local database management, which will be replaced with **PostgreSQL/MySQL** later if scaling is needed.

### 2. **Infrastructure Provisioning (IaC)**
Using **Terraform**, all infrastructure resources will be provisioned in **AWS**, including EC2 instances, security groups, and load balancers.

### 3. **Containerization (Docker)**
The application will be containerized using **Docker** to ensure consistency across different environments (development, staging, production).

### 4. **CI/CD Pipeline**
The CI/CD pipeline will be implemented using **GitHub Actions** to:
- **Build** Docker images.
- **Test** the application.
- **Deploy** to **AWS** after manual approval.

### 5. **Deployment**
The application will be deployed in a redundant setup on **AWS EC2 instances**. The application will be accessible through a **reverse proxy (Nginx)**, and communication will be secured using **Let's Encrypt** for SSL/TLS.

### 6. **Monitoring**
Basic monitoring and logging will be set up to monitor application performance and health using **AWS CloudWatch** (instead of Prometheus/Grafana for simplicity).

---

## Infrastructure Architecture

### Cloud Hosting: AWS
The infrastructure will be hosted on **AWS**, leveraging EC2 instances for hosting the application and related services.

### Resource Allocation
Resources like EC2 instances and security groups will be allocated using **Terraform**. The system will use a **Load Balancer** for traffic distribution.

### Services to be Set Up
- **AWS EC2 instances** for hosting the application.
- **Elastic Load Balancer (ELB)** for traffic routing.
- **Nginx** for reverse proxying and SSL termination.
- **RDS** or EC2-managed database (if scaling is required).

### Environment Differentiation
- **Development Environment**: Local Docker containers or lightweight EC2 instances.
- **Production Environment**: Full-scale, redundant AWS setup with load balancing.

---

## Decisions and Rationale

- **AWS** is chosen for its scalability, ease of use, and integration with Terraform.
- **SQLite** is initially used for simplicity, with the potential to scale to **PostgreSQL/MySQL** later.
- **Docker** ensures that the application runs consistently in all environments.
- **Terraform** is used to automate infrastructure provisioning, following IaC best practices.
- **Nginx** is selected for reverse proxying, with **Let’s Encrypt** providing SSL/TLS certificates.
- **GitHub Actions** automates the build, test, and deployment pipeline.

---

## Conclusion

This project provides a scalable and automated infrastructure for deploying the **Student Management System** application. Using **AWS**, **Terraform**, and **Docker**, we can deploy and manage the application efficiently. With **GitHub Actions** for CI/CD, the application can be continuously integrated and deployed, ensuring a smooth development lifecycle. The use of **Nginx** and **Let’s Encrypt** will secure the application through HTTPS.
