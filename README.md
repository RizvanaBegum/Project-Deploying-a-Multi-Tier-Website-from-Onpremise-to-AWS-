# Deploying a Multi-Tier Website Using AWS EC2

## Project Overview
This project demonstrates the deployment of a multi-tier PHP-based web application using **Amazon Web Services (AWS)**. The solution leverages **Amazon EC2** for scalable computing, **Amazon RDS** for database management, and **Auto Scaling** to ensure high availability and handle variable traffic loads.

## Problem Statement
**Company ABC** wanted to move their on-premises **PHP-based website** and **MySQL database** to AWS to improve scalability and availability. The company required automatic scaling to handle traffic spikes and ensure the system remains highly available.

## Solution Architecture
The architecture consists of three tiers:
- **Web Tier (EC2)**: Hosts the PHP-based web application and handles HTTP traffic.
- **Application Tier (EC2)**: Scales automatically based on traffic to ensure high availability.
- **Database Tier (RDS MySQL)**: Stores data for the application, ensuring data durability and availability.

The solution uses **AWS Auto Scaling** to automatically add or remove EC2 instances based on load, and **Amazon RDS** to manage the MySQL database.

## Steps to Deploy

### 1. Launch EC2 Instances
- Launch an EC2 instance to host the PHP website.
- Configure the instance to handle HTTP and SSH traffic.

### 2. Set Up Auto Scaling
- Enable Auto Scaling to ensure a minimum of 2 EC2 instances are always running.

### 3. Create an RDS Instance
- Launch an **Amazon RDS MySQL** instance.
- Ensure the RDS instance is in a private subnet and can only be accessed by the application tier.

### 4. Configure the Database
- Create a MySQL database named `intel` and a table named `data`.
- Secure the database with a password: `intel123`.

## Key Technologies
- **Amazon EC2**: For hosting the web and application tiers.
- **Amazon RDS (MySQL)**: For managing the database.
- **AWS Auto Scaling**: To handle varying traffic demands.
- **VPC & Security Groups**: To control access and ensure security.

## Architecture Diagram
![image](https://github.com/user-attachments/assets/bc87c7e0-3376-4b43-ab17-e098b73f4936)


## How to Run the Project
1. Clone the repository to your local machine.
2. Deploy the **CloudFormation** template (if using).
3. Follow the deployment steps outlined above.

## Project Benefits
- **Scalability**: Automatically scales up or down based on traffic demands.
- **High Availability**: Auto Scaling ensures continuous availability of the web application.
- **Resilient Data**: The RDS instance is preserved, even if the infrastructure stack is deleted.

## Conclusion
This project showcases how to deploy a scalable, high-availability web application using AWS services. By leveraging EC2, Auto Scaling, and RDS, the system ensures performance and reliability under varying traffic conditions.

## Contact
For any questions or further assistance, please contact:

- *Name*: Rizvana Begum
- *Email*: rizvanabegumt@outlook.com
- *LinkedIn*: www.linkedin.com/in/rizvanabegum
