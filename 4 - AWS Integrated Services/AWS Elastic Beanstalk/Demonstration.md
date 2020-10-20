# Starting Elastic Beanstalk for a Web Application

1. Go to **Compute** > **Elastic Beanstalk**
2. Click **Create New Application**
   * Enter application name
   * Enter application description
3. Create the environment
   1. Select the environment
      * Choose a web server environment or worker environment for long working tasks
   2. Enter the domain you want to use or it will be auto-filled
   3. Enter the environment description
   4. Choose the platform to match your code i.e. Python, Node.js
   5. Upload your code
      1. Choose file from system
      2. Choose S3 URL
   6. Label the environment version
   7. Modify Default Configurations if needed
      * Can choose price model, etc.
4. Create the AWS Beanstalk environment
   * Takes 5 - 10 mins maybe more
