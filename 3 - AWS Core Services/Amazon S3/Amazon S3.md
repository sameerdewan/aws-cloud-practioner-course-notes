# Amazon Simple Storage Service (S3)

* **Amazon Simple Storage Service (S3)** is a fully managed storage service that provides a simple API for *storing and retrieving data*
* Data stored in S3 is not associated with any particular server and you do not have to manage any infrastructure yourself
* You can store virtually unlimited **objects**, Amazon S3 holds trillions of objects and regularly peaks at millions of requests per second
* **Objects** can be almost any data file, such as images, videos, or server logs
* Since objects can even be TBs in size, even *database snapshots* can be stored as objects
* S3 offers low latency access via HTTP/HTTPS from anywhere at any time
* You can access S3 *privately through a private cloud endpoint*
* You can exercise fine grained control over who can access your data using **Identity and Access Management policies**, **bucket policies**, and even manage **per-object based access control lists**.
* By default, no data is shared publicly
* Data can be encrypted in tranist and you can choose to enable server side encryption on objects
* In S3, you can create a bucket to hold your data
* To create an object, the data needs a key to access the object later
* The common format for this key (type string) is a filepath i.e. `media/sam.mp3`
* When a bucket is created, it is associated with an **AWS Region**
* When stored in buckets, *data is reduntantly stored across multiple AWS facilities within your selected region*
* AWS S3 is meant to provide durability even with concurrent data loss across facilities
* S3 automatically scales and manages storage behind your bucket as the data inside your bucket grows
* Data storage increases as application needs increase
* S3 scales to handle a high volume of requests
* With S3, you do not have to provision storage or throughput, and you will only be billed for what you use
* You can access Amazon S3 through the **AWS Management Console**, **AWS CLI**, or **AWS SDKs**
* You can access data in a bucket directly via the rest endpoints (HTTP/HTTPS)


| Bucket Name | Region Specific Endpoint | Object Key |
| - | - | - |
| https://examplebucket/ | s3-us-west-2.amazonaws.com/ | media/sam.mp3 |

* Bucket names must be globally unique and DNS compliant
* Object keys should use URL safe characters

> ### Common Use Cases
>
> 1. Storing Application Assets
>    * Access through traditional servers, Amazon EC2, or anything else
>    * Server Logs
>    * Other application files needing to be stored
>    * You can offload serving the content from your application to S3, allowing your clients to directly fetch data from S3
> 2. Static Web Hosting
>    * S3 buckets can serve up static contents of your website i.e. *HTML*, *JavaScript*, *CSS*, etc.
> 3. Backup and Disaster Recovery
>    * The high durability of S3 makes it a good candidate to store backups of data
>    * Can be set up to support cross region replication
> 4. Staging Area for Big Data
>    * Can be used by data software
>    * Can import and export data
>
