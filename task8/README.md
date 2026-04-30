# Task: S3 Bucket Access Control (Public + Restricted Access)

## Objective
Create an S3 bucket, configure public access, and restrict access to specific IAM users and IP addresses.

---

## Steps

### 1. Create S3 Bucket
- Created a new S3 bucket  
- Verified bucket settings  

---

### 2. Configure Public Access
- Disabled Block Public Access (if required)  
- Added bucket policy to allow public read access  

---

### 3. Restrict Access (Users + IPs)
- Modified bucket policy to:
  - Allow access only to specific IAM users  
  - Restrict access based on IP address condition  
- Used conditions like:
  - `aws:SourceIp` for IP restriction  
  - IAM user ARN for identity restriction  

---

### 4. Apply Policy
- Saved and applied updated bucket policy  
- Verified permissions  

---

## Output

- S3 bucket created successfully  
- Public access enabled  
- Access restricted to specific IAM users  
- Access limited to allowed IP addresses  
- Secure and controlled access implemented  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)