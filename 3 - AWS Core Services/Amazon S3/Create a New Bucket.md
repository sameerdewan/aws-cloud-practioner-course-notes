# Create a New Bucket, Add Data, and Retrieve Data

1. From **Amazon S3**, click **+ Create Bucket**
   * You will be prompted to set a bucket name, and select a **region**
   * The bucket name must be DNS compliant
   * Select a region close to your EC2 instance, or where you need it located for regulatory or business purposes
   * You can change permissions and versions, or leave it default
   * Your bucket should be created
2. **AWS CLI** upload data
   * From folder `folder/demo.txt`
   * `terminal$ aws s3 cp demo.txt s3://bucket-name//hello.txt`
   * You can also take the contents of a folder and sync it, uploading the files in the folder if they do not already exist in th destination bucket
   * `terminal$ aws s3 sync folder s3://bucket-name/files`
   * You can sync an **EC2 instance** folder to an S3 bucket as well
