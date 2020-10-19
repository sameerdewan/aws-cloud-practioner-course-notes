# Application Load Balancer Demo

1. Start in **AWS Management Console** > **EC2 Console**
2. View **Instances** and confirm running
3. **Load Balancers** > **Load Balancers**
4. Click **Create Load Balancer**
5. Select Default Application Load Balancer
6. Click **Continue**
7. Configure the Load Balancer
   1. Name the Load Balancer
   2. Name will go into the DNS endpoint
   3. Default listener has an HTTP at port 80
   4. Add another listener, HTTP at port 443
   5. Select the Availability Zone
      * Two Availability Zones are required with subnets created for the instances
   6. You can then tag your load balancer key/value
8. Configure the Security Settings
   * If using SSL listener only
9. Configure Security Group
   * Select Default or Your own
10. Configure the Routing
    1. Configure routing rule for backend destination for load balancer
    2. Name the target group
    3. Choose the protocol
    4. Choose the port
    5. Choose the Protocol and path for health check settings
11. Click Register Targets
    1. Choose what instances you want to be hit
    2. Add to registered
12. Review
    * See all configurations and confirm
13. Click **Create**
14. Load balancer should be successfully created
15. To register a second target, go under **Load Balancer** > **Target Group**
16. Click **Create Target Group**
    1. Choose group name
    2. Choose the port
    3. Choose the VPC
    4. Choose the health check protocol
    5. Choose the health check path
    6. Under advanced health check settings
       * Lower interval to 10s or as needed
17. Successfully create second target group
18. Make sure you register the correct instance as a target for that second target group
19. Go to Load Balancer
20. Verify both ports set up for listening on Load Balancer
21. To forward the instance to port 443, click **View and Edit Rules**, forward to the correct target group
22. To test, copy DNS name
    1. Paste DNS name, go to target set up for container 1 and confirm container 1
    2. Paste DNS name 2, go to target set up for container 2 and confirm container 2
