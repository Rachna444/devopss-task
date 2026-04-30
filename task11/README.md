# Task: EC2 Policy – Allow Start/Stop BUT Deny in Specific Region

## Objective
Allow EC2 start and stop actions while restricting these actions in a specific AWS region.

---

## Steps

### 1. Open IAM Console
- Navigated to IAM → Policies  
- Clicked on Create Policy  

---

### 2. Configure Permissions
- Allowed actions:
  - `ec2:StartInstances`
  - `ec2:StopInstances`  
- Added condition to deny these actions in a specific region (e.g., `ap-south-1`)  

---

### 3. Attach Policy
- Attached policy to required IAM user/role  

---

### 4. Apply & Verify
- Saved policy  
- Tested start/stop actions in different regions  

---

## Output

- EC2 start/stop allowed in permitted regions  
- Actions denied in restricted region  
- Region-based restriction enforced  
- Policy working as expected  

---

## Screenshots

![Output](screenshots/image.png)