# How to Build and Configure an EC2 Instance

Overview

> 1. Login to the **AWS Console**
> 2. Choose a **Region** where to host your **Instance**
> 3. Launch the **EC2 Wizard**
> 4. Select an **Amazon Machine Image** (AMI)
>    - Software (SW) platform for the Instance
> 5. Select Instance type
>    * Harware (HW) referring to hardware capabilities
> 6. Configure Network
> 7. Configure Storage
> 8. Configure key pairs which will allow us to connect to the Instance
> 9. Launch and Connect to the Instance

Detailed

> 1. Login to the **AWS Console**
>    * Set the **Region** (close to where you need the **Instance** served or for regulatory needs)
>    * From top navigation, click **Services**
>    * Under **Compute**, click **EC2**
>    * Click **Launch Instance**
>    * Choose the **Amazon Machine Image** (AMI) that will be the software load that comes with the instance once it is launched
>    * Under **Quick Start**, choices for AMIs include **Windows** and **Linux** servers
>    * The **AWS Marketplace** has third party images available for choosing as well
>    * Under **My AMIs**, we can select some of our own built images
> 2. Select the Hardware (HW) selection also known as the **Instance type**
> 3. Configure Instance Details
>    * You can select the # of instances
>    * Network configuration can be set here
> 4. Add and Set Storage Device Settings
>    * You can select the size of the root volume and change the type of disk
>    * You can also add new volumes
>    * You can choose to delete a volume on termination or deletion of the instance
> 5. Add Tags
>    * Tags consist of a case sensitive key value pair, for example: *Key = Name, Value = Webserver*
>    * A copy of a tag can be applied to volumes, instances, or both
>    * Tags will be applied to all instances and volumes
> 6. Configure a Security Group
>    * A security group is a set of firewall rules
>    * Automatically creates a default rule for SSH connectivity
>    * You can add more rules, for example: *HTTP to allow for web connectivity*
>    * You can name and give a description to a security group
> 7. Review Instance Launch Details
>    * Provides an overview to remind you of selections made in previous steps
>    * In order to connect to the Instance using SSH, you need a key pair
> 8. From the provided dropdown, you can choose from:
>    * Choose existing key pair
>    * Create new key pair
>    * Proceed without key pair
> 9. Name the key pair created and download the private key
>    * The private key is **absolutely required** to connect over SSH
> 10. Launch Instance
>     * You will be provided with an instance identifier
> 11. To connect to the instance, you need the Public DNS (IPv4) address
> 12. You can use **PuTTY** to connect to your instance
>     1. Enter the Public DNS (IPv4) address in PuTTY
>     2. Under Connection > SSH > Auth browse for the downloaded private key
>     3. PuTTY may require a *.ppk* file on Windows, in which case you must convert your *.pem* file using PuTTY-gen
>     4. You can now login to your instance and work via the terminal
