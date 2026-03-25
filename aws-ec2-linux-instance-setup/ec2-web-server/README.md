EC2 Web Server Deployment on AWS\

Project Objective
This project demonstrates the end-to-end process of provisioning a Linux-based EC2 instance on AWS, configuring secure access via SSH, deploying an Apache web server, and exposing the application over the internet using a public IP address.

Services and Tools Used:
- AWS EC2 (Elastic Compute Cloud)
- Security Groups (Network Access Control)
- Ubuntu Server 22.04 LTS
- Apache HTTP Server
- SSH (Secure Shell)
 
Implementation Details:
1. EC2 Instance Provisioning
Launched a t2.micro (Free Tier eligible) instance
Selected Ubuntu Server 22.04 LTS as the operating system
Configured a key pair (.pem) for secure authentication
2. Network Configuration (Security Groups)
Type	Port	Source	Purpose
SSH	22	My IP	Secure administrative access
HTTP	80	0.0.0.0/0	Public web access
3. Secure Access via SSH
ssh -i ec2-keypairs.pem ubuntu@13.60.85.131

Successfully established a secure remote connection to the EC2 instance.

4. Web Server Installation and Configuration
sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
5. Service Verification
sudo systemctl status apache2

The service status confirmed that Apache was active and running.

6. Application Deployment
echo "Hello from EC2 - Sanyam Project" | sudo tee /var/www/html/index.html

A custom web page was deployed to validate server functionality.

7. Application Access

The application was accessed via:

http://13.60.85.131

The deployed web page was successfully rendered in the browser.

8. Instance Lifecycle Management
The EC2 instance was stopped after testing to prevent unnecessary resource consumption and billing.
Architecture Overview
User (Web Browser)
        ↓
Public IP (EC2 Instance)
        ↓
Security Group (Ports 22, 80)
        ↓
EC2 Instance (Ubuntu + Apache Web Server)

Screenshots:
1. EC2 instance in running state
2. Security group inbound rules configuration
3. SSH session confirmation
4. Apache service status (running)
5. Deployment command execution
6. Web application output in browser
7. Instance stopped state

(All screenshots are available in the screenshots/ directory.)

Key Outcomes:
- Gained hands-on experience with cloud infrastructure provisioning
- Implemented secure remote access using SSH key-based authentication
- Deployed and managed a production-grade web server
- Configured network access controls using AWS Security Groups

Author
Sanyam
