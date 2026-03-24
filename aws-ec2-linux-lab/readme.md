# Remote Server Access Setup on AWS EC2

## Project Objective
This project demonstrates the process of provisioning a Linux-based EC2 instance on AWS and establishing secure remote access using SSH.

---

## Services and Tools Used
- AWS EC2 (Elastic Compute Cloud)  
- Security Groups  
- Ubuntu Server  
- SSH (Secure Shell)  
- MobaXterm  

---

## Implementation Steps

### 1. EC2 Instance Provisioning
- Launched an Ubuntu-based EC2 instance (t2.micro)  
- Configured key pair (.pem) for authentication  

---

### 2. Security Group Configuration
- Allowed SSH (Port 22) from My IP  
- Allowed HTTP (Port 80) for web access  
- Allowed HTTPS (Port 443) for secure communication  

---

### 3. Remote Access via SSH
- Connected to the EC2 instance using MobaXterm  
- Authenticated using the generated key pair  

---

## Outcome
- Successfully provisioned a cloud-based Linux server  
- Established secure remote access using SSH  
- Validated connectivity and instance availability  

---

## Key Learnings
- Understanding of EC2 instance lifecycle  
- Secure access using SSH key-based authentication  
- Basic network configuration using security groups  
