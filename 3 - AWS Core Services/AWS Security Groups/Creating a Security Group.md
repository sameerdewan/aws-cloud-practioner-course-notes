# Creating a Security Group

1. Log into the **AWS Management Console**
2. Click **Compute** -> **EC2**
3. **Network and Security** -> **Security Groups**
4. Click **Create Security Group**
   * Enter the name of the security group
   * Enter the description of the security group
   * Enter the rules for the security group
   * *By default, all inbound traffic is denied, and all outbound traffic is allowed*
5. Edit Inbound and Outbound rules here
6. You can edit rules by:
   * **Type**
   * **Protocol**
   * **Port Ranges**
   * **Source**
7. *The best practice is to figure out what traffic is required for your instance, and specifically only allow that traffic*

# Creating a Web Server Security Group

> Continuation of steps from above

1. Enter the name for example `web-server-sg`
2. Enter the description for example `Allow web traffic`
3. Select a **VPC**
4. Under type, select `HTTP`, source `0.0.0.0/0`
5. Under type, select `HTTPS`, source `0.0.0.0/0`
6. With this setup, all of the Internet is allowed to interact with this security group
7. Click **Create**
8. `web-server-sg` should be created

> Defining good security groups is necessary for security compliance.
