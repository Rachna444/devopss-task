# Task: S3 Policy – Allow All Buckets BUT Deny One Specific Bucket

## Objective
Provide full access to all S3 buckets while restricting access to one specific bucket.

---

## Steps

### 1. Open IAM Console
- Navigated to IAM → Policies  
- Clicked on Create Policy  

---

### 2. Configure Permissions
- Allowed full S3 access (`s3:*`)  
- Added explicit deny for one bucket (`restricted-bucket-name`)  

---

### 3. Attach Policy
- Attached policy to required IAM user/role  

---

### 4. Apply & Verify
- Saved policy  
- Tested access on multiple buckets  

---

## Output

- Full access granted to all S3 buckets  
- Access denied for specified bucket  
- Deny rule overrides allow  
- Policy enforced successfully  

---

## Screenshots

![Output](screenshots/image.png)