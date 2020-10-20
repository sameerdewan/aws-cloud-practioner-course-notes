# AWS CloudFormation Demo

> **Goals**
>
> 1. Open CloudFormation via the Amazon Management Console
> 2. Open the CloudFormation Designer
> 3. Create a new template
> 4. Add entries to create a new VPC to the template
> 5. Create a new stack using the new template
> 6. View the new VPC resource

1. Open **AWS Management Console** -> **CloudFormation**
   1. Create a Stack (**Create New Stack**)
   2. You can load or design a new template
2. Use the **CloudFormation Designer**
   1. To the left are resource types that can be dragged onto the template area that build out our template
   2. Drag the **VPC** into the grid
   3. Notice the template being built in JSON/YAML below
   4. Add in the *CIDR block which is the network address*
   5. Click properties and add CIDR block with the address `10.0.0.0/16`
3. Click **Create Stack**
4. You can select the template, noticing that it was added to an **S3 bucket**
5. Click **Next**
6. Name the stack
7. Click **Next**
8. Tags can be added
9. Permissions can be added
10. Click **Next**
11. Summary Screen
    * Click **Create**
12. Go and view the **Stacks**
    * The stack should be created with the state *CREATE_COMPLETE*
13. Head to **Services** -> **VPC**
    * Confirm the **VPC** was *created*
