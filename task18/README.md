# Task: Terraform VPC Setup (Public + Private Subnets, IGW, NAT Gateway, Route Tables)

## Objective
Create a secure AWS networking architecture using Terraform with:
- VPC
- Public Subnet
- Private Subnet
- Internet Gateway
- NAT Gateway
- Route Tables

---

## Objects Created

- VPC (10.0.0.0/16)
- Public Subnet (10.0.1.0/24)
- Private Subnet (10.0.2.0/24)
- Internet Gateway
- Elastic IP (for NAT)
- NAT Gateway
- Public Route Table
- Private Route Table
- Route Table Associations

---

## Important Concepts (Short Notes)

- **VPC** → Isolated network in AWS  
- **Public Subnet** → Direct internet access via Internet Gateway  
- **Private Subnet** → No direct internet access  
- **NAT Gateway** → Allows private subnet outbound internet only  
- **Route Tables** → Control traffic flow inside VPC  

---

## Flow Architecture

- Public Subnet → Internet Gateway → Internet  
- Private Subnet → NAT Gateway → Internet (outbound only)

---

##  Output

- VPC successfully created  
- Public subnet has internet connectivity  
- Private subnet secured (no direct inbound internet)  
- NAT Gateway enables secure outbound access  
- Route tables correctly associated with subnets  
- Fully working Terraform-based network setup  

---

## 📸 Screenshots

![Output](screenshots/image.png)   

---