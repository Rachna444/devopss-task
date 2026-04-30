# Task: Multi-Environment AWS Infrastructure using Terraform

## Objective
Provision AWS resources dynamically for multiple environments using Terraform:
- S3 buckets per environment
- Conditional versioning
- IAM users from multiple environments
- Dynamic IAM policies per environment
- Policy attachment per user
- Lifecycle rules using dynamic blocks
- Remote backend configuration (S3 + DynamoDB)

---

## Steps

### 1. Create S3 Buckets using `for_each`
- Created multiple S3 buckets for environments  
- Naming format:
  - `myapp-<env>-<bucket_suffix>`  
- Used `for_each` to loop through environments  

---

### 2. Enable Versioning Conditionally
- Used `aws_s3_bucket_versioning` resource  
- Enabled versioning only when:
  - `versioning = true`  

---

### 3. Create IAM Users from Multiple Environments
- Combined user lists from all environments  
- Removed duplicates using Terraform functions  
- Created IAM users dynamically  

---

### 4. Create Dynamic IAM Policies
- Generated IAM policies per environment  
- Restricted access to only that environment’s bucket  
- Used `jsonencode()` for policy creation  

---

### 5. Attach Policies to Users
- Attached environment-specific policies  
- Ensured users can access only their assigned bucket  

---

### 6. Lifecycle Rules using Dynamic Block
- Added lifecycle rules dynamically  
- Configured rules per environment  
- Managed storage transitions and expiration  

---

### 7. Remote Backend Configuration
- Configured Terraform backend:
  - S3 for state storage  
  - DynamoDB for state locking  
- Ensured safe collaboration and state management  

---

## Output

- S3 buckets created per environment using `for_each`  
- Versioning enabled conditionally  
- IAM users created dynamically without duplicates  
- Environment-specific IAM policies enforced  
- Access restricted per environment bucket  
- Lifecycle rules applied dynamically  
- Remote backend configured (S3 + DynamoDB)  
- Fully modular and production-ready Terraform setup  

---

## Screenshots

![Output](screenshots/image.png)