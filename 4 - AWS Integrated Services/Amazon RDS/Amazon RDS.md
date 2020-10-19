# Amazon Relational Database Services  (RDS)

> **Challenges of running our own Relational Databases including several administrative tasks:**
>
> * Server Maintenance
> * Energy Footprint
> * Software Install
> * Patches
> * Database Backups
> * High Availability
> * Limits on Scalability
> * Data security
> * Operating System (OS) installs
> * Operating System (OS) patches

* AWS provides a service to provide this without ongoing adminstration -  **Amazon Relational Database Services** (RDS)
  * RDS automates time consuming tasks
  * RDS scales
  * We can focus on *application optimization rather than database optimization*
  * Offload all the above operational challenges to Amazon
  * A database instance is an isolated environment which can contain numerous databases
* You can tailor your performance and cost to your database needs
* Specify your database wanted, Amazon RDS supports the following databases:
  * MySQL
  * Amazon Aurora
  * Microsoft SQL Server
  * PostgreSQL
  * MariaDB
  * ORACLE
* You can run an instance of RDS using an **Amazon VPC**
  * *Database instance isolated to a private subnet are only allowed to be targeted by allowed applications*
* **RDS automatically seeds a copy to a standby copy db in another Availability Zone, synchronously**
* **RDS automatically brings standby db to master on master failure**
  * Nothing changes in our code at this event of master failure by using **DNS**
* Read replicas for MySQL, MariaDB, PostgresSQL and Amazon Aurora available
  * Offloading read queries from master instance are ideal for read heavy database workloads that are heavy
  * This offloading helps scale out beyond capacity contraints of single db instance
  * Read dbs can be made master, but must be done manually, which can also acts as another level of disaster protection
  * This can also help with offloading and faster delivery

> **Use Cases**
>
> * Web Applications
>   * High throughput
>   * Massive storage scalability
>   * High Availability
> * E-commerce Applications
>   * Low cost database
>   * Data security
>   * Fully managed solution
> * Mobile and Online Games
>   * Rapidly grow capacity
>   * Automatic scaling
>   * Database monitoring

* Amazon RDS manages our database infrastructure

> **Benefits**
>
> * Highly scalable
> * High performnace
> * Easy to adminster
> * Available and Durable
> * Secure and Compliant
