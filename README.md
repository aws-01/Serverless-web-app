🚀 Serverless Web App on AWS

A fully serverless student management web application built using AWS cloud services.

This project demonstrates how to build and deploy a scalable application without managing any servers.

🏗️ Architecture Flow
Frontend (S3 - index.html + scripts.js)
        ↓
API Gateway
        ↓
AWS Lambda (Python Functions)
        ↓
DynamoDB
☁️ AWS Services Used

Amazon S3 – Static website hosting

Amazon API Gateway – REST API endpoint

AWS Lambda – Backend logic using Python

Amazon DynamoDB – NoSQL database

IAM – Roles & Permissions management

📂 Project Structure
Serverless-web-app/
│
├── index.html                # Frontend UI
├── scripts.js                # API integration logic
├── insertStudentData.py      # Lambda function to insert data
├── getStudents.py            # Lambda function to fetch data
└── README.md
⚙️ Features

Add student data to DynamoDB

Retrieve student records

Fully serverless backend

No EC2 / No server maintenance

Auto scaling architecture

Cost-efficient design

🔧 How It Works

User opens website hosted on S3

Frontend calls API Gateway endpoint

API Gateway triggers Lambda function

Lambda interacts with DynamoDB

Data is returned back to frontend

🧠 What I Learned

Serverless architecture fundamentals

Lambda function creation using Python

API Gateway integration

DynamoDB CRUD operations

IAM roles and security best practices

Real-time cloud deployment experience

📈 Future Improvements

Add authentication (Cognito)

Add CloudFront for CDN

Implement CI/CD using GitHub Actions

Add logging & monitoring using CloudWatch