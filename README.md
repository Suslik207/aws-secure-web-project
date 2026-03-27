#  Secure AWS Web Application

##  Project Description
This project demonstrates how to deploy and secure a basic web application in AWS.  
The goal was to understand core cloud security concepts such as IAM roles, least privilege, and secure network configuration.

---

##  Architecture
- EC2 (t3.micro - Free Tier)
- IAM Role
- S3
- VPC (custom)
- Security Groups
- CloudTrail (logging)

---

##  What I Did
- Created a custom VPC with subnet and internet access
- Launched EC2 instance (t3.micro)
- Configured SSH access securely (restricted to my IP)
- Installed and configured nginx web server
- Deployed a simple HTML website
- Created and attached IAM Role to EC2
- Enabled secure access from EC2 to S3 (without access keys)
- Enabled CloudTrail for monitoring and logging

---

##  Security Features
- IAM Role used instead of access keys
- Applied least privilege principle
- Restricted SSH access (port 22) to my IP only
- Allowed HTTP (port 80) for public web access
- No sensitive credentials stored on the server
- CloudTrail enabled for auditing activity

---

##  What I Learned
- Difference between IAM User and IAM Role
- Why IAM roles are more secure than access keys
- Basics of cloud network security (VPC, Security Groups)
- How to reduce risk using least privilege
- How EC2 interacts with S3 securely
- Importance of logging and monitoring in cloud environments

---

##  Security Decisions

- IAM Role was used instead of access keys to avoid credential exposure
- SSH access was restricted to minimize attack surface
- Least privilege principle was applied to reduce potential blast radius

---

##  Notes
This project was created as part of my learning path towards becoming a Cloud Security Engineer.

---

##  Screenshots

### EC2 Instance
!<img width="1919" height="877" alt="my instance" src="https://github.com/user-attachments/assets/cc53e39a-b4cb-4f65-a569-fb1cfe3eceb0" />

### Security Group
!<img width="1919" height="878" alt="security groups" src="https://github.com/user-attachments/assets/756cb615-30c6-45a9-ba13-af2fc776d506" />

### IAM Role
!<img width="1900" height="876" alt="IAM Role Png" src="https://github.com/user-attachments/assets/4baea16d-9da7-4edd-9cd0-2444c8c178a0" />

### Web Application
!<img width="1917" height="881" alt="my secure-web" src="https://github.com/user-attachments/assets/aee3b709-5d51-4d1f-81fc-f4c6e0e4a712" />


