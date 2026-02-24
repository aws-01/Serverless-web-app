# 🚀 Serverless Web Application on AWS

A fully serverless student management web application built using Amazon Web Services (AWS).  
This project demonstrates how to design and deploy a scalable cloud-native application without managing any servers.

---

## 🚀 Features

- 📝 Add Student Records – Insert student data into the database  
- 📋 View Students – Retrieve and display stored student records  
- ⚡ Serverless Backend – No EC2 instances or server maintenance  
- 🔄 Auto Scaling – Automatically scales based on demand  
- 🔐 Secure Access – IAM roles and permission-based access control  
- 💰 Cost Efficient – Pay only for what you use  
- ☁️ Cloud-Native Architecture – Built entirely using AWS managed services  

---

## 🧰 Technologies Used

| Category | Technology |
|-----------|-------------|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python (AWS Lambda) |
| Database | Amazon DynamoDB |
| API Layer | Amazon API Gateway |
| Cloud Platform | Amazon Web Services (AWS) |
| Storage | Amazon S3 |
| Security | IAM Roles & Policies |
| Version Control | Git & GitHub |
| Tools | VS Code |

---

## ☁️ AWS Architecture Overview

### 🪣 Amazon S3 (Simple Storage Service)

- Hosts the static frontend (index.html, scripts.js)
- Static website hosting enabled
- Acts as the entry point for users

### 🔗 Amazon API Gateway

- Creates REST API endpoints
- Connects frontend requests to Lambda functions
- Handles request and response management

### ⚡ AWS Lambda

- Executes backend Python code
- Two Lambda functions:
  - insertStudentData.py – Inserts data into DynamoDB
  - getStudents.py – Fetches student records
- Automatically scales based on traffic

### 🗄️ Amazon DynamoDB

- Fully managed NoSQL database
- Stores student records
- High availability and low latency

### 🔐 IAM (Identity and Access Management)

- Configured roles for Lambda to access DynamoDB
- Followed least-privilege security model
- Ensures secure resource access

---

## 🏗️ Architecture Flow

User Browser  
↓  
Amazon S3 (Frontend Hosting)  
↓  
API Gateway (REST API)  
↓  
AWS Lambda (Python Functions)  
↓  
Amazon DynamoDB (Database)

---

## 📂 Project Structure

Serverless-web-app/  
│  
├── index.html                # Frontend UI  
├── scripts.js                # API integration logic  
├── insertStudentData.py      # Lambda function to insert data  
├── getStudents.py            # Lambda function to fetch data  
└── README.md  

---

## 🔧 Deployment Steps

1. Created S3 bucket and enabled static website hosting  
2. Uploaded frontend files  
3. Created DynamoDB table  
4. Developed Lambda functions in Python  
5. Integrated Lambda with API Gateway  
6. Configured IAM roles and permissions  
7. Tested API endpoints  
8. Connected frontend to API Gateway  

---

## 🧠 What I Learned

- Serverless architecture design principles  
- AWS Lambda & API Gateway integration  
- DynamoDB CRUD operations  
- IAM role-based security  
- Cloud deployment best practices  
- Building scalable and cost-efficient systems  

---

## 📈 Future Improvements

- Add authentication using Amazon Cognito  
- Add CloudFront for CDN performance  
- Implement CI/CD using GitHub Actions  
- Add monitoring using CloudWatch  
- Improve validation and error handling  

---
