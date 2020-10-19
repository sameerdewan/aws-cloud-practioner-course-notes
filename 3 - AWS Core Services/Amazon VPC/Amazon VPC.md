# Amazon Virtual Private Cloud (VPC)

* The **AWS Cloud** offers *pay-as-you-go*, *on demand compute*, as well as managed services all accessible via the web
* These compute resources and services must be accessible via normal IP protocols and implemented with familiar network structure
* Customers need to adhere to networking best practices as well as meet regulatory and organizational requirements
* **Amazon Virtual Private Cloud** (Amazon VPC) is the networking AWS Service that will meet our networking requirements
* Amazon VPC allows us to create a *private network* in the AWS Cloud while using the *same concepts as on premise networking*, all while *abstracting much of the complexity*, without sacrificing *control*, *usability*, and *security*.
* Allows complete control of network configuration
  * configs: *IP Address bases*, *subnets*, and *routing tables*
  * Control what you expose to the Internet and what you isolate to the Amazon VPC
* You can deploy your VPC in a way to layer security controls in the network
  * Isolating subnets
  * Defining access controls and lists
  * Customizing routing tables
  * Complete control over when to allow both incoming and outgoing traffic
* Other AWS Services that deploy into your VPC inherit and take advantage of the security that you build into your cloud network
* AWS VPC is a foundational service and integrates with numerous AWS Services

> ##### Services AWS VPCs can integrate with
>
> * AWS EC2
> * AWS OpsWork
> * Amazon S3
> * Amazon EMR
> * Amazon EFS
> * Amazon DynamoDB
> * Amazon RDS
> * AWS Elastic Beanstalk
> * Amazon ElastiCache
> * Amazon Workspaces
> * Amazon Route 53
> * Elastic Load Balancing
> * AWS Data Pipeline
