# Task: S3 Bucket Policy (Restricted Uploads + Security Controls)

## Objective
Configure an S3 bucket policy to:
- Allow uploads only to `uploads/` folder  
- Deny object deletion  
- Deny uploads without server-side encryption  
- Enable versioning  

---

## Steps

### 1. Create S3 Bucket
- Created a new S3 bucket  
- Configured basic settings  

---

### 2. Enable Versioning
- Enabled versioning from bucket properties  
- Ensures object history and recovery  

---

### 3. Configure Bucket Policy

Applied policy rules:
- Allow `PutObject` only for `uploads/` prefix  
- Deny `DeleteObject` for all objects  
- Deny uploads without server-side encryption (SSE)  

---

### 4. Apply Policy
- Attached bucket policy  
- Verified permissions  

---

## Output

- Uploads allowed only inside `uploads/` folder  
- Delete operations blocked completely  
- Unencrypted uploads rejected  
- Versioning enabled successfully  
- Secure S3 storage configured  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)