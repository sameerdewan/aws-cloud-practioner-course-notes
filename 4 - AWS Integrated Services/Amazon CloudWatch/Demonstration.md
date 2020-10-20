# Create a CloudWatch Events Rule

1. Go to the [CloudWatch console](https://console.aws.amazon.com/cloudwatch/)
   1. Under **Alarms**, click **Events**
   2. Click **Create Rule**
   3. Select an event source
      1. **Event Pattern**
      2. **Event Schedule**
      3. Schedule can be at a fixed rate
         * Cron job syntax is usable here
      4. You can log the state of an **EC2 Instance** using **CloudWatch Events**
      5. Create a **Lambda function** to log the state change events
      6. Create a rule to run your Lambda function whenever you launch an EC2 Instance
      7. Choose **Add Target** and then choose **Lambda function**
      8. For function, *select* the Lambda function that you created
2. Set up a **CloudWatch Alarm** for the EC2 Instance
   1. **Instances** -> **Instances** -> **Actions** -> **CloudWatch Monitoring** -> **Add/Edit Alarms** *or* **CloudWatch** -> **Alarms** -> **Create Alarm**
   2. Select recipients, actions, topics
   3. **Create** the CloudWatch Alarm
3. Create a **CloudWatch Dashboard**
4. Select graph to add to dashboard for metric observation
