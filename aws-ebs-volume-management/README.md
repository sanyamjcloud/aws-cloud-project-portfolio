# AWS EBS Volume Attachment for Persistent Storage

## Problem Statement
In cloud environments, compute instances are ephemeral, but application data must persist.  
This project demonstrates how to configure AWS EBS volumes to ensure data durability independent of the EC2 instance lifecycle.

---

## Architecture Overview
EC2 Instance  <---->  EBS Volume (Persistent Storage)

---

## Tech Stack
- AWS EC2
- AWS EBS (gp3)
- Linux (Ubuntu/Amazon Linux)
- SSH

---

## Implementation

1. Created a 5GB gp3 EBS volume in the same availability zone as the EC2 instance  
2. Attached the volume to the running instance  

3. Verified the device:
```bash
lsblk
```

4. Formatted the volume:
```bash
sudo mkfs -t ext4 /dev/xvdf
```

5. Mounted the volume:
```bash
sudo mount /dev/xvdf /data
```

6. Verified mount:
```bash
df -h
```

7. Configured persistence across reboots using `/etc/fstab`

---

## Validation

- Restarted the EC2 instance  
- Verified automatic remount of the volume  
- Confirmed that stored data remained intact after reboot  

---

## Key Learnings

- Difference between ephemeral and persistent storage in cloud environments  
- Importance of `/etc/fstab` for automated mounting  
- Handling storage at OS level in cloud infrastructure  

---

## Screenshots

- EBS volume attached (AWS Console)  
- Terminal output (`lsblk`, `df -h`)  

---

## Author
Sanyam Jain
