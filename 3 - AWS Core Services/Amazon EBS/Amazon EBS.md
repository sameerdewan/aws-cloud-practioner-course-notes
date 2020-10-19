# Amazon Elastic Block Store (EBS)

* **EBS volumes** can be used as a *storage unit* for **EC2 instances**
* Whenever you need disk space for our instances running on AWS, we can think about using EBS
* These volumes can be hard disks (HDD) or SDD devices which you pay for as you use
* Whenever a volume is not needed anymore, it can be deleted and you can stop paying for it
* Persistent and customizable block storage for EC2 instances
* Replicated in the same **availability zone** as the EC2 instance it is used as a storage unit for
* Backups are created using snapshots
* Offers easy and transparent encryption
* Elastic volumes
* EBS volumes are designed to be durable and available, data in volumes are automatically replicated across multiple servers running in the availability zone
* EBS is much more durable than HDD or SDD because of the block-level replication
* When creating an EBS volume, you can choose the type that best suits your needs
* A database can be configured to use a secondary volume for the data, which may perform faster than the volume assigned to the operating system
* A magnetic volume can be used for logs, as magnetic is cheaper
* Amazon EBS gives us the ability to create **point-in-time snapshots of our volumes** and **recreate a volume from a snapshot** anytime
* We can share and copy snapshots to a different **AWS Region** for even greater *disaster recovery protection*
* Encryption on EBS volumes at no additional cost
* EC2 -> EBS containers can be encrypted in transit
* EBS volumes have the ability to increase capacity and change to different types *i.e. hard disk (HDD) -> SDD or increasing a 50GB volume to a 16TB* volume **on the fly** **without needing to stop the instances**
