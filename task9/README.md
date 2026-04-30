# Task: EC2 Policy – Allow All Actions BUT Deny Termination

## Objective
Allow all EC2 operations while preventing instance termination.

---

## Steps

### 1. Open IAM Console
- Navigated to IAM → Policies  
- Clicked on Create Policy  

---

### 2. Configure Permissions
- Allowed all EC2 actions (`ec2:*`)  
- Added explicit deny for termination (`ec2:TerminateInstances`)  

---

### 3. Attach Policy
- Attached policy to required IAM user/role  

---

### 4. Apply & Verify
- Saved policy  
- Tested permissions on EC2 instance  

---

## Output

- All EC2 actions allowed (start, stop, reboot, etc.)  
- Instance termination blocked  
- Deny rule overrides allow  
- Policy enforced successfully  

---

## Screenshots

![Output](screenshots/image.png)