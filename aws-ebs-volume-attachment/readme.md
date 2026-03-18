# AWS EBS Volume Attachment Project

## Overview
This project demonstrates how to create a 5GB EBS volume and attach it to a Linux EC2 instance in the same availability zone.

## Objective
To understand AWS block storage creation and attachment process.

## Services Used
- Amazon EC2
- Elastic Block Store (EBS)

## Configuration
Volume Size: 5GB  
Volume Type: gp3  
Availability Zone: Same as instance  

## Steps Performed
1. Created EBS volume
2. Selected correct availability zone
3. Attached volume to Linux instance
4. Verified attachment status

## Result
The volume was successfully attached to the EC2 instance and its state changed to "In-use".

## Key Learning
EBS volumes must be created in the same availability zone as the instance to attach successfully.

## Author
Sanyam Jain
