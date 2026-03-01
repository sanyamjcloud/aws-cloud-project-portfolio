# AWS Launch Template Deployment

## Overview

This project demonstrates the process of creating and using an AWS Launch Template to deploy multiple Linux EC2 instances with predefined configuration settings. The objective is to automate infrastructure provisioning so that identical instances can be launched quickly and consistently.

---

## Objective

To create a launch template capable of deploying four Linux EC2 instances with predefined security group rules allowing SSH, HTTP, and HTTPS access.

---

## Services Used

* Amazon EC2
* Launch Templates
* Security Groups

---

## Configuration

**Instance Settings**

* Operating System: Amazon Linux
* Instance Type: t2.micro
* Instance Count: 4
* Key Pair: Configured

**Security Group Rules**

| Protocol | Port | Access   |
| -------- | ---- | -------- |
| SSH      | 22   | My IP    |
| HTTP     | 80   | Anywhere |
| HTTPS    | 443  | Anywhere |

---

## Implementation Steps

1. Created a security group allowing ports 22, 80, and 443.
2. Created a launch template specifying AMI, instance type, and key pair.
3. Attached the security group to the launch template.
4. Launched instances using the template configuration.
5. Set the instance count to four.
6. Verified that all instances were successfully running.

---

## Result

Four EC2 instances were launched simultaneously with identical configurations and security settings. The deployment confirmed that launch templates can be used to standardize and automate instance provisioning.

---

## Conclusion

The project demonstrates practical knowledge of AWS infrastructure deployment using launch templates. This approach is useful in real-world environments where rapid and consistent server deployment is required.

---

## Author
Sanyam Jain
