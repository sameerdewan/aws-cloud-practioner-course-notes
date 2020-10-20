# Creating an SNS Topic

1. From the SNS Dashboard, create a new topic - the creation of a topic allows us to send necessary information to the destinations I wish to send it to
   1. Enter the topic name
   2. Enter the topic display name
   3. Click **Create Topic**
2. **Topic Actions** > **Check Topic Policy**
   1. Security option - specific users publish to the topic
   2. Security option - specific users subscribe to the topic
   3. Select delivery protocols
      1. HTTP
      2. Email-JSON
      3. Application
      4. HTTPS
      5. SMS
      6. AWS Lambda
      7. Email
      8. Amazon SQS
   4. Click **Update Policy**
   5. Create a subscription by clicking **Create Subscription**
      1. Choose the protocol
      2. Create the endpoint
      3. Click **Create Subscription**
   6. The subscription is now pending confirmation
   7. Confirm the subscription to remove the pending state
   8. Go to an **Amazon S3 bucket**, which can generate information to send to the created SNS topic
      1. **Bucket** -> **Properties** -> **Enroll to event**-> **Add an event **-> **SNS topic**
      2. Amazon S3 bucket is now a **publisher**
      3. Every time object created or deleted, information will now be sent to the SNS topic, which is received by **subscribers**
      4. Click **Save**
