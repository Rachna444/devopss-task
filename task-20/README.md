📘 Task — Deploy EC2 with Nginx using Terraform
🎯 Objective

The goal of this task was to:

Launch an EC2 instance using Terraform
Install and start Nginx automatically
Make the web server accessible over the internet
🛠️ Steps Performed
1️⃣ EC2 Instance Creation
Created an EC2 instance using Terraform
Selected a suitable Amazon Machine Image (AMI)
Chose instance type (e.g., t2.micro)
2️⃣ Security Group Configuration
Created a security group
Allowed inbound traffic:
Port 22 (SSH)
Port 80 (HTTP)
Allowed all outbound traffic
3️⃣ Nginx Installation (User Data)
Used user data script to automate setup
Installed Nginx during instance launch
Started and enabled Nginx service
Deployed a simple HTML page
4️⃣ Output Configuration
Configured Terraform output to display public IP
Used this IP to access the web server

##screenshot
![Output](screenshots/image1.png)  
![Output](screenshots/image2.png)
