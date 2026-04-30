# Task: EC2 + Web App + AMI + Launch Template + Auto Scaling Group

## Objective
Deploy a web application on EC2, create an AMI from it, and use it to configure a Launch Template and Auto Scaling Group with scaling policy.

---

## Steps

### 1. Launch EC2 Instance
- Created EC2 instance  
- Selected OS (Amazon Linux / Ubuntu)  
- Allowed SSH (22) and HTTP (80) in security group  
- Assigned public IP  

---

### 2. Install Web Application
- Connected to EC2 via SSH  
- Installed web server (Nginx/Apache)  
- Added application files to web directory  
- Verified app using browser  

---

### 3. Create AMI (Image)
- Selected EC2 instance  
- Created image (AMI)  
- Waited until AMI becomes available  

---

### 4. Create Launch Template
- Created Launch Template  
- Selected created AMI  
- Configured instance type, key pair, and security group  

---

### 5. Configure Auto Scaling Group
- Created Auto Scaling Group using Launch Template  
- Selected VPC and subnets  
- Set desired, minimum, and maximum capacity  

---

### 6. Configure Scaling Policy
- Added scaling policy  
- Based on CPU utilization threshold  
- Auto scale out/in based on load  

---

## Output

- EC2 instance running web application  
- AMI created successfully  
- Launch Template configured using AMI  
- Auto Scaling Group deployed  
- Automatic scaling working based on policy  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)  
![Output](screenshots/image3.png)  
![Output](screenshots/image4.png)  
![Output](screenshots/image5.png)