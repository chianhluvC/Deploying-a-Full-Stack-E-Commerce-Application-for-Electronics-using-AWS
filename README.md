
# 🚀 Deploying a Full-Stack Electronics E-Commerce Website with AWS

This repository contains materials and instructions for a workshop on deploying a full-stack e-commerce web application (built with Spring Boot) to AWS. The deployment utilizes essential AWS services such as EC2, S3, RDS, and Route 53.

## 🌐 Demo

Workshop link: [workshop.huyanh.click](https://workshop.huyanh.click)  
Deployed website link: [workshop.huyanh.click](https://workshop.huyanh.click)

> ✅ AWS is a powerful cloud platform that provides flexible and scalable solutions for hosting enterprise-grade applications like Spring Boot-based e-commerce systems.

---

## 🧱 Deployment Architecture

Below is the architecture overview of deploying a Spring Boot-based e-commerce application using EC2, S3, and RDS on AWS:

```
[ User ] 
   ↓
[ Route53 Domain ]
   ↓
[ EC2 Instance (Spring Boot App) ]
   ↓                    ↘
[ RDS (MySQL/PostgreSQL) ]   [ S3 (Static content / Backup / Assets) ]
```

---

## 📚 Table of Contents

1. [Introduction](#1-introduction)
2. [Preparation](#2-preparation)
3. [Deployment](#3-deployment)
4. [Conclusion & Future Development](#4-conclusion--future-development)
5. [Clean Up Resources](#5-clean-up-resources)

---

## 1. Introduction

- Overview of the project: build an electronics e-commerce system using Spring Boot
- Introduction to AWS services used:
  - **EC2**: Run the backend application (Spring Boot)
  - **S3**: Store images or static files
  - **RDS**: Store relational database (MySQL/PostgreSQL)
  - **Route 53**: Set up a custom domain

---

## 2. Preparation

- [x] Create an **S3 bucket**
- [x] Allocate an **Elastic IP** for EC2
- [x] Launch an EC2 instance (Amazon Linux 2 or Ubuntu)
- [x] Create an RDS instance (MySQL/PostgreSQL)
- [x] Buy a domain using Route 53 & point to the Elastic IP
- [x] Download the source code and build the `.jar` file

---

## 3. Deployment

- Upload the `.jar` file to S3
- SSH into the EC2 instance and download the `.jar` from S3
- Configure the EC2 instance to run the Spring Boot application (using `tmux`, `screen`, or `systemd`)
- Set up database connection with RDS (DB_HOST, USER, PASSWORD…)
- Access the domain or IP to test the application

---

## 4. Conclusion & Future Development

- Comparison with other deployment methods:
  - Elastic Beanstalk, ECS, Lambda...
  - Heroku, Vercel, Netlify, Railway
- Suggestions for further improvements:
  - CI/CD with GitHub Actions or AWS CodePipeline
  - Security enhancements (HTTPS, IAM Role, Secrets Manager)
  - Monitoring & Logging with CloudWatch, AWS X-Ray

---

## 5. Clean Up Resources

To avoid unnecessary costs, remove the following resources after the workshop:

- [ ] Delete RDS instance
- [ ] Delete S3 bucket
- [ ] Terminate EC2 instance and release Elastic IP
- [ ] Delete the domain (if purchased for testing)

---

## 📎 Contact / Q&A

If you have any questions or encounter issues during the workshop, feel free to create an issue or contact the trainer for support.

---

> 🛠 This workshop is designed as a practical example to help you understand how to deploy a full-stack Spring Boot application on AWS infrastructure.
