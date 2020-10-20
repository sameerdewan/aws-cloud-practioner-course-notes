# Amazon CloudWatch

* **Amazon CloudWatch** monitors your **Amazon Web Services **(AWS) resources and the applications you run on AWS in real time
* Collect and track metric
  * CPU utilization
  * Data transfer
  * Disk I/O and Utilization
* Collect and monitor log files
* Set **Alarms** (a core feature of CloudWatch)
  * Send notifications
  * Take other automated actions
* Automatically react to changes
  * System wide visibility into resource utilization, application performance, and operational health
* **Amazon CloudWatch Architecture**
  * **CloudWatch Metrics**
    * CPU utilization
    * Status checks
  * Reported to the **AWS Management Console**
  * Can be collected and sent to fire a **CloudWatch Alarm**
  * Can send an sms/email or auto scaling event

> Use Cases for Amazon CloudWatch
>
> * Respond to state changes in your AWS resource
> * Automatically invoke an AWS Lambda function to update DNS entries when an event notifies that Amazon EC2 instance enters the Running state
> * Direct specific API records from CloudTrail to a Kinesis stream for detailed analysis of potential security or availability risks
> * Take a snapshot of an Amazon EBS volume on a schedule
> * Log S3 Object Level Operations using CloudWatch Events

* Amazon CloudWatch Components
  * Metrics
    * Data about the performance of the systems
    * Represents a time-ordered set of data points that are published to CloudWatch
    * By default, several services provide free metrics for resources
      * Such as **Amazon EC2 instances**, **Amazon EBS volumes**, and **Amazon RDS DB instances**
    * Publish your own application metrics for an additional fee
    * Load all the metrics in your account for search, graphing, and alarms
  * Alarms
    * Watches a single metric
    * Performs one or more actions
      * Based on the value of the metric relative to a threshold over a number of time periods
        * i.e. an **EC2 Instance** -> start, stop, terminate, reboot
        * **Auto Scaling Action** -> Launch an Autoscaling Configuration -> Add more instances to application pool, remove instances from application pool
        * Send a message to an **SNS topic**
        * **Only sustained state changes trigger actions**
  * Events
    * Near real-time stream of system events that describe changes in AWS resources
    * Use simple rules to match events and route them to one or more target functions or streams
    * Aware of operational changes as they occur
    * Responds to these operational changes and takes corrective action as necessary
    * Schedule automated actions that self-trigger at certain times using Cron or rate expressions
  * Logs
    * Monitor and troubleshoot systems and applications using existing log files
      * Monitor logs for specific phrases, values, or patterns
    * Retrieve the associated log data from **CloudWatch Logs**
    * Includes an installable agent for Ubuntu, Amazon Linux, and Windows at no additional charge
    * Monitor Logs from **Amazon EC2 Instances** in real time
    * Monitor **AWS CloudTrail Logged Events**
    * Archive Log Data
    * Store and Monitor Application Log Files
      * Metrics can be stored durably in **CloudWatch as CloudWatch Logs**
        * Admins and other parties can review CloudWatch logs directly in the **AWS Management Console**
        * *Logs can be stored in Amazon S3*, to be accessed by other services or another user
        * *Logs can be streamed in real through solutions like Amazon Kinesis Streams or AWS Lambda to take further action on a particular metric*
  * Dashboards
    * Customizable home pages in the CloudWatch console to monitor your resources in a single view
      * Even resources that are spread across different regions
    * Create customized views of the metrics and alarms for your AWS resources
      * Each dashboard can display multiple metrics and can be accessorized with text and images
    * Create dashboards by using the **AWS Management Console**, the **AWS CLI**, or by using the **PutDashboard API**
