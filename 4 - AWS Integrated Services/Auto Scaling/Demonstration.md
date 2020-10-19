# Auto Scaling Demonstration

> ##### Goals
>
> 1. Create a Launch Configuration
> 2. Create an Auto Scaling Group
> 3. Create an Auto Scaling Policy
> 4. Trigger Auto Scaling

1. **Autoscaling** > **Autoscaling Groups**
2. **Create Auto Scaling Group**
3. Create **Launch Configuration**
4. Choose **Amazon Machine Image** (AMI)
5. Name the Launch Configuration
6. Set the Storage Settings
7. Set the Security Groups Settings
8. Click **Launch Configuration**
9. Choose key pair or create new
10. Create Launch Configuration
11. You will be taken to set the properties for the auto scaling group
12. Name the group
13. Specifiy starting instance amount
14. Specify the VPC and subnet to deploy instances into
15. Configure the Scaling Policies
    1. Set scaling between min and max or keep at initial size
    2. Choose a target tracking value for the policy
       * Target tracking is the simplest way to get started with auto scaling policies
    3. Create the auto scaling groups
16. View auto scaling groups to confirm the created auto scaling group exists
17. To trigger auto scaling, edit the group details and change the minimum number of instances in the configuration to be higher than what is set
18. It will autoscale and launch the difference (n) in instances
19. *TL;DR* - Auto scaling allows us to maintain performance and minimize cost while we sleep
