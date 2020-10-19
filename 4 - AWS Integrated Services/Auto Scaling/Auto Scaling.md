# Auto Scaling

* **Auto Scaling** helps you ensure that you have the correct number of **Amazon EC2** instances available to*handle the load for your application*
* Removes the guess work of meeting work load requirements
* It is critical to monitor performance using**Amazon CloudWatch**
* CloudWatch*will not scale our EC2 instances*
* We do not want to under utilize resources nor do we want to under perform for our end users
* Auto Scaling lets us scale*based on criteria we specify*
* Maintain performance and minimize cost
* **Scalability**
  * Ensure workload has enough EC2 resources to meet fluctuating perfromance requirements
  * **Scaling out** and**Scaling in** based on conditions we define
  * Scaling out > adds instances
  * Scaling in > terminates instances
  * To create auto scaling, you need three auto scaling components**Launch Configuration**,**Auto Scaling Group**, and**Auto Scaling Policy**

| Auto Scaling Component | Definition |
| - | - |
| Launch Configuration | Defines what will be launched by auto scaling, such as choosing an  **Amazon Machine Image** (AMI), instance type, security groups, roles. The things you think about when you create an EC2 instance. |
| Auto Scaling Group | Defining where a deployment takes place and boundaries for the deployment. Define which **VPC** to deploy instances, and which **Load Balancer** to interact with. We set boundaries for a group. We can set a minimum of instances, and maximum of instances. We can set a desired capacity, which is our number of instances to start with. |
| Auto Scaling Policy | Specification of when to create/terminate EC2 instances. We can schedule or create thresholds to do this. |

* **Automation**
  * Automate EC2 resource provisioning to occur on demad
* **Dynamic Auto Scaling**
  * Create**CloudWatch alarms** based on performance by EC2 instance or load balancer
  * When a defined*threshold* is crossed, a*CloudWatch alarm triggers an auto scaling event which will either scale out or scale in EC2 instances*
* Alarms
  * Create a threshold for CPU Utilization and consecutive period of time defined
  * Define an action
* Typically, create a scale out event alarm and create a scale in event alarm

