Project Verification Document
------------------------------

Project Title:
AWS EBS Volume Attachment to Linux EC2 Instance

Objective:
To create a 5GB Elastic Block Store (EBS) volume and attach it to a running Linux EC2 instance within the same Availability Zone.

Verification Steps Performed:

1. Confirmed EC2 instance was in Running state.
2. Verified selected Availability Zone of instance.
3. Created a 5GB EBS volume in the same Availability Zone.
4. Checked volume status changed to "Available".
5. Attached volume to the selected EC2 instance.
6. Verified volume state changed to "In-use".
7. Confirmed attachment from EC2 console storage section.

Result:
The volume was successfully created and attached to the Linux EC2 instance without errors.

Validation Evidence:
Refer to screenshots folder for visual proof of:
- Volume creation
- Availability state
- Attachment configuration
- In-use status

Conclusion:
The task was completed successfully and demonstrates correct understanding of AWS EBS volume provisioning and attachment requirements.

Status:
Completed
