📘 Task — Implement Failover Routing
🎯 Objective

The goal of this task was to:

Ensure high availability across regions
Deploy a primary Application Load Balancer (ALB) in one region
Deploy a secondary (backup) ALB in another region
Configure health checks
Enable automatic failover using DNS routing
🛠️ Steps Performed
1️⃣ Primary ALB (Region A)
Created an Application Load Balancer in Region A
Attached target group (EC2 instances / backend services)
Configured listener (HTTP/HTTPS)
2️⃣ Secondary ALB (Region B)
Created another ALB in a different region (Region B)
Configured with same setup as primary
Acts as backup in case of failure
3️⃣ Health Checks Configuration
Configured health checks for both ALBs
Monitored application endpoints (e.g., /health)
Ensured only healthy targets receive traffic
4️⃣ DNS Failover Setup
Used Amazon Route 53 for routing
Created two records:
Primary record → Region A ALB
Secondary record → Region B ALB
Enabled Failover Routing Policy
5️⃣ Automatic Failover
Route 53 continuously checks health of primary ALB
If primary becomes unhealthy:
Traffic automatically redirected to secondary ALB
No manual intervention required
📸 Screenshots (to add)
ALB in Region A
ALB in Region B
Target groups health status
Route 53 hosted zone records
Health check configuration
✅ Result
Multi-region failover successfully implemented
High availability achieved
Automatic traffic switching during failure
Improved reliability and fault tolerance
## screenshot
![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)  
![Output](screenshots/image3.png)  
![Output](screenshots/image4.png)  
![Output](screenshots/image5.png)