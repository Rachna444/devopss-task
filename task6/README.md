# Task: Bastion-less Architecture using Session Manager

## Objective
Eliminate the need for a Bastion Host by securely accessing private EC2 instances using AWS Systems Manager Session Manager.

---

## Steps

### 1. EC2 Setup (Private Instance)
- Launched EC2 instance in private subnet  
- Disabled public IP assignment  
- Configured security group (no SSH from internet)  

---

### 2. Remove Bastion Host
- Terminated existing Bastion EC2 instance  
- Ensured no SSH access from public network  

---

### 3. Configure IAM Role
- Created IAM role for EC2  
- Attached policy: `AmazonSSMManagedInstanceCore`  
- Attached role to private EC2 instance  

---

### 4. Systems Manager Setup
- Verified SSM Agent is installed and running  
- Confirmed instance appears in Systems Manager → Managed Instances  

---

### 5. Connect via Session Manager
- Opened Systems Manager → Session Manager  
- Started session with private EC2 instance  
- Accessed instance without SSH or public IP  

---

## Output

- Bastion host removed successfully  
- Private EC2 instance has no public access  
- IAM role configured for SSM access  
- Instance managed via Systems Manager  
- Secure connection established using Session Manager  
- No SSH keys or open ports required  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)