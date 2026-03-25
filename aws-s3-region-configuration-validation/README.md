AWS EBS Cross Region Volume Attachment Test

Project Objective
To create a 5GB EBS volume in a different region than an existing Linux EC2 instance and verify whether attachment is possible.

Services Used
- Amazon EC2
- Elastic Block Store (EBS)

Concept Tested
EBS volumes are region-specific resources and cannot be attached to instances in different regions.

Architecture
Linux Instance → Mumbai Region
Volume → Singapore Region

Result
Volume creation succeeded.
Attachment failed because instance exists in another region.

Outcome
Successfully demonstrated AWS regional resource limitation.
