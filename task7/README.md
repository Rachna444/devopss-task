# Task: Path-Based Routing using Application Load Balancer (ALB)

## Objective
Configure an Application Load Balancer to route traffic based on URL paths:
- `/videos` → Videos Target Group  
- `/images` → Images Target Group  

---

## Steps

### 1. Setup EC2 Instances
- Launched EC2 instances for:
  - Videos service  
  - Images service  
- Installed web server (Nginx/Apache)  
- Deployed respective content  

---

### 2. Create Target Groups
- Created target groups:
  - Videos-TG → for videos instances  
  - Images-TG → for images instances  
- Configured health checks  

---

### 3. Create Application Load Balancer
- Created ALB  
- Attached to VPC and public subnets  
- Configured listener on HTTP (port 80)  

---

### 4. Configure Listener Rules
- Added path-based routing rules:

  - If path = `/videos*` → forward to Videos-TG  
  - If path = `/images*` → forward to Images-TG  

- Set default rule (optional fallback target group)  

---

## Output

- ALB successfully configured  
- `/videos` path routed to Videos target group  
- `/images` path routed to Images target group  
- Traffic distributed correctly based on URL path  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)