There are three aws accounts considered for this POC.
Source which has the S3 Bucket and IAM Role which has access to this bucket. 
Shared account which has IAM Role which assumes the Source IAM Role. 
Destination account which has the Lambda and IAM Role which is the Lambda Execution role which is trying to read the contents of files from S3 bucket present in the source. 
The destination IAM Roles double assumes to get the S3 data from Source AWS Account to Destination AWS account with the help of IAM Role present in the Shared AWS Account.
