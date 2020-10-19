# Create a New Volume and Attach it to an EC2 Instance

> 1. **Go to the AWS Management Console**
>    * Under **Elastic Block Store** -> **Volumes** to view EBS volumes
>    * To create and attach an EBS volume to an EC2 instance, **it must be located in the same availability zone as the EC2 instance**
> 2. Create Volume
>    * Under **Volumes**, click **Create Volume**
>    * Use the same availability zone as the EC2 instance
>    * SSD will charge for the amount in size GB
>    * We can also restore a snapshot to a volume here
>    * We can also add encryption and tags here
>    * Click **Create Volume**
> 3. From **Elastic Block Store** -> **Volumes**
>    * From the **Actions** dropdown, select **Attach Volume**
>    * Specify the **instance ID or name tag** for the instance
>    * Specify a **device**
>    * Click **Attach**
> 4. Log into the **EC2 Instance** that we attached the **EBS volume** to
>    * In the **Amazon Mangement Console**, go to **Instances** -> **Instances**
>    * Select the instance that we attached the EBS Volume to
>    * Click **Connect**
>    * Copy the SSH command and paste it in your terminal
>    * You will connect to the EC2 Instance through the terminal
>    * Run `lsblk` to list block storage devices attached to the instance
>    * You will be able to se the created EBS disk
>    * With the EBS volume attached to the EC2 Instance, **we can create a file system with it**
>    * Run the command (*example*: `sudo mk2fs /dev/xvdb`)
>    * The Linux operating system will **create the file system**
>    * You can now **mount the volume** into a folder on the Linux Machine
>    * To mount, run (*example:* `sudo /dev/xvdb /mnt`)
>    * This will mount the volume in the **/mnt** folder
>    * We can now use this as a storage block, creating directories and moving files into those directories
>    * To unmount, run (*example:* `unmount /mnt`)
>    * Then go to **Elastic Block Store** > **Volumes** in the **Amazon Management Console**
>    * In the **Actions** dropdown click **Detach Volume**, which will move the volume to the *available* state, which can be *reattached now to another instance*
>    * You can add tags i.e. database volume, as **tags are important for drilling into AWS billing and discerning the cost for volumes with a particular tag in a certain period of time**
>    * Tags can be applied to everything that support tags, including EC2 Instances
>    * *The benefits of using Amazon EC2 instances compared to a physical server in your infrastructure are the ability to have different storage requirements and paying only for the capacity you use*
>
