# Task: S3 Policy – Deny Deletion BUT Allow Everything Else

## Objective
Allow all S3 operations while preventing deletion of objects.

---

## Steps

### 1. Open IAM Console
- Navigated to IAM → Policies  
- Clicked on Create Policy  

---

### 2. Configure Permissions
- Allowed all S3 actions (`s3:*`)  
- Added explicit deny for delete actions (`s3:DeleteObject`)  

---

### 3. Attach Policy
- Attached policy to required IAM user/role  

---

### 4. Apply & Verify
- Saved policy  
- Tested delete and other S3 operations  

---

## Output

- All S3 actions allowed (upload, read, update, etc.)  
- Delete operation blocked  
- Deny rule overrides allow  
- Policy enforced successfully  

---

## Screenshots

![Output](screenshots/image.png)