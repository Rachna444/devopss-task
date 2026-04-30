# Task: Private EC2 with S3 Access via VPC Endpoint

## Objective
Allow a private EC2 instance to access S3 using a VPC Gateway Endpoint while removing internet access (no NAT Gateway).

---

## Steps

### 1. VPC & EC2 Setup
- Created VPC with private subnet  
- Launched EC2 instance in private subnet  
- No public IP assigned  

---

### 2. Remove Internet Access
- Ensured no NAT Gateway present  
- Route table does not have internet route (0.0.0.0/0 → IGW/NAT)  

---

### 3. Create VPC Gateway Endpoint (S3)
- Created Gateway VPC Endpoint for S3  
- Attached endpoint to VPC  
- Associated with private subnet route table  

---

### 4. Route Table Configuration
- Verified route added:
  - S3 prefix list → VPC Endpoint  
- No default internet route present  

---

### 5. IAM Role for EC2
- Attached IAM role with S3 access permissions  
- Allowed required S3 actions (read/write as needed)  

---

### 6. Validation (CLI)
- Connected to EC2 instance  
- Tested S3 access:
  ```bash
  aws s3 ls

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)