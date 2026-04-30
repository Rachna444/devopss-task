# Task: Implement IAM Best Practices

## Objective
Improve security by organizing users into groups, applying least privilege access, enabling MFA, and restricting S3 access using custom policies.

---

## Steps

### 1. Create IAM Groups
- Created IAM groups:
  - Admin
  - Dev
  - ReadOnly  

---

### 2. Apply Least Privilege
- Assigned policies based on role:
  - Admin → Full access  
  - Dev → Limited service access  
  - ReadOnly → Read-only permissions  

---

### 3. Enable MFA (Root User)
- Enabled Multi-Factor Authentication for root account  
- Configured authenticator app  

---

### 4. Custom S3 Policy
- Created custom IAM policy  
- Allowed access only to specific S3 folder (restricted path)  
- Attached policy to required group/user  

---

## Output

- IAM groups created successfully  
- Least privilege access enforced  
- Root account secured with MFA  
- S3 folder-level restricted access implemented  
- Overall account security improved  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)  
![Output](screenshots/image3.png)