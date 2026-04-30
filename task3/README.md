# Task: CloudWatch Monitoring Setup

## Objective
Set up monitoring and alerting using Amazon CloudWatch for EC2 and ALB, with SNS notifications.

---

## Steps

### 1. Enable EC2 Detailed Monitoring
- Selected EC2 instance  
- Enabled detailed monitoring (1-minute metrics)  

---

### 2. Create CPU Utilization Alarm
- Opened CloudWatch → Alarms  
- Created alarm on EC2 CPU Utilization  
- Defined threshold and evaluation period  

---

### 3. Configure SNS Notification
- Created SNS topic  
- Subscribed email to topic  
- Linked SNS topic to CloudWatch alarm  

---

### 4. Monitor ALB Metrics
- Selected Application Load Balancer  
- Viewed metrics in CloudWatch  
- Monitored request count, latency, and target health  

---

## Output

- Detailed monitoring enabled for EC2  
- CPU utilization alarm configured successfully  
- SNS notifications triggered on threshold breach  
- ALB metrics actively monitored  
- End-to-end monitoring and alerting working  

---

## Screenshots

![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)