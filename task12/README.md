# Task: VPC Policy – Allow VPC Creation BUT Deny Internet Gateway Creation

## Objective
Allow users to create VPCs while restricting the creation of Internet Gateways.

---

## Steps

### 1. Open IAM Console
- Navigated to IAM → Policies  
- Clicked on Create Policy  

---

### 2. Configure Permissions
- Allowed VPC-related actions (e.g., `ec2:CreateVpc`)  
- Added explicit deny for Internet Gateway creation (`ec2:CreateInternetGateway`)  

---

### 3. Attach Policy
- Attached policy to required IAM user/role  

---

### 4. Apply & Verify
- Saved policy  
- Tested VPC and Internet Gateway creation  

---

## Output

- VPC creation allowed  
- Internet Gateway creation blocked  
- Deny rule overrides allow  
- Policy enforced successfully  

---

## Screenshots

![Output](screenshots/image.png)