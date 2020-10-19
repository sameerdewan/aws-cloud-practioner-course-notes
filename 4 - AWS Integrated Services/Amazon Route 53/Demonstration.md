# Creating a Hosted Zone Configuring a Record Set

1. Own a domain name
2. Go to **Route 53** > **Hosted zones**
3. Click **Create Hosted Zone**
   * Enter the domain name
   * Enter the comment,
   * Enter the type (public, private)
4. On creation, the hosted zone will be created
5. On the hosted zone, click **Create a Record Set**
6. You can then assign sub domains that resolve to an IP address of an **EC2 instance**, **S3 endpoints**, etc.
7. Choose a **routing policy**
8. Hit **Create**
9. Route 53 will then resolve the domain to that instance IP if we check in our browsers by searching our domain name
10. By running `nslookup www.nameofapp.net` we can get the IP address and confirm it resolves to our IP address of EC2 instance/S3 endpoint/etc.
11. Queries are automatically routed to the closest **AWS Edge Location**
12. This provides higher availability and performance at volume
13. Route 53 also offers
    * Simple Routing
    * Geo-location
    * Failover
    * Weighted round robin
    * Latency based
    * Multi-value answer
