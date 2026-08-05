---
title: "Project Proposal"
date: 2026-06-22
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

This section summarizes the proposed workshop that will be implemented during the internship.

# EduWallet
## Personal Finance Management System on AWS

### 1. Executive Summary

EduWallet is a personal finance management application designed for students to record income and expenses, manage monthly budgets, and monitor their spending habits.

The system is planned to be deployed on Amazon Web Services (AWS) using a lightweight cloud architecture that focuses on security, reliability, and ease of deployment. The project aims to provide hands-on experience with AWS while demonstrating how cloud services can be used to build a practical web application.

---

### 2. Problem Statement

#### Current Problems

Many students still manage their personal finances manually using notebooks or spreadsheets. This approach has several limitations:

- Difficult to track daily income and expenses.
- No centralized data storage.
- Difficult to access financial records across devices.
- Limited budgeting and spending analysis.
- Poor scalability when the number of users increases.

#### Proposed Solution

EduWallet provides a cloud-based personal finance management system deployed on AWS.

Users can securely log in, manage transactions, upload receipt images, and store financial data in a centralized database. The system also provides basic monitoring to ensure stable operation.

#### Expected Benefits

- Easy financial management.
- Secure user authentication.
- Reliable cloud storage.
- Practical experience in deploying cloud applications.
- Foundation for future AI-powered financial analysis.

---

### 3. Solution Architecture

The project follows a simple three-tier architecture consisting of:

- Presentation Layer
- Application Layer
- Database Layer

**Architecture Diagram**

![EduWallet Architecture](/images/AWS_EduWallet.drawio.png)

### AWS Services

- **Amazon EC2**
  - Hosts the backend application.

- **Amazon RDS PostgreSQL**
  - Stores user accounts and financial data.

- **Amazon S3**
  - Stores receipt images uploaded by users.

- **Amazon Cognito**
  - Handles user authentication and authorization.

- **Amazon CloudWatch**
  - Collects logs and monitors application performance.

### Component Design

- Users access EduWallet through a web browser.
- Authentication is handled by Amazon Cognito.
- The backend application runs on Amazon EC2.
- Transaction data is stored in Amazon RDS PostgreSQL.
- Receipt images are stored in Amazon S3.
- Amazon CloudWatch monitors logs and system health.

---

### 4. Technical Implementation

#### Implementation Phases

The project is divided into four phases:

1. Requirement Analysis
   - Identify system requirements.
   - Design database schema.

2. Infrastructure Preparation
   - Launch Amazon EC2.
   - Configure Amazon RDS.
   - Configure Amazon S3.
   - Configure Amazon Cognito.

3. Application Development
   - Develop backend APIs.
   - Connect the database.
   - Implement authentication.
   - Implement image upload.

4. Testing and Documentation
   - Functional testing.
   - Deployment verification.
   - Documentation completion.

#### Technical Requirements

- AWS Account
- Amazon EC2
- Amazon RDS PostgreSQL
- Amazon S3
- Amazon Cognito
- Amazon CloudWatch
- Visual Studio Code
- Git & GitHub

---

### 5. Timeline

| Week | Activities |
|------|------------|
| Week 1 | Learn AWS fundamentals and prepare development environment |
| Week 2 | Learn IAM, VPC, and system networking |
| Week 3 | Learn database services and architecture |
| Week 4 | Learn Amazon S3 and storage services |
| Week 5 | Learn application deployment concepts |
| Week 6 | Analyze EduWallet requirements and architecture |
| Week 7 | Complete proposal and system design |
| Week 8 | Implement workshop and finalize documentation |

---

### 6. Estimated Budget

The project mainly uses AWS Free Tier during development.

| AWS Service | Estimated Monthly Cost |
|-------------|----------------------:|
| Amazon EC2 | Free Tier |
| Amazon RDS PostgreSQL | Free Tier |
| Amazon S3 | Free Tier |
| Amazon Cognito | Free Tier |
| Amazon CloudWatch | Free Tier |

**Estimated Total:** Approximately **USD 0–10/month** during development.

---

### 7. Risk Assessment

#### Potential Risks

- Incorrect AWS configuration.
- Unexpected AWS charges.
- Data loss.
- Unauthorized access.

#### Mitigation Strategy

- Follow AWS Best Practices.
- Enable AWS Free Tier monitoring.
- Perform regular database backups.
- Apply IAM least-privilege principles.

#### Contingency Plan

- Restore data from database backups.
- Redeploy the application if deployment fails.
- Monitor system health using Amazon CloudWatch.

---

### 8. Expected Outcomes

#### Technical Outcomes

- Deploy a cloud-based personal finance management system.
- Apply AWS services in a real-world project.
- Understand cloud deployment workflows.
- Gain practical experience with AWS.

#### Future Development

Future versions of EduWallet may include:

- AI-powered spending analysis.
- Financial reports and dashboards.
- Monthly budget recommendations.
- Mobile application support.