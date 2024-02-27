# sagemaker

we can either create notebook instance or use sagemaker studio

# AWS services:

- S3 bucket
- SageMaker
- SageMaker studio

# save model in S3 bucket and read it through Sagemaker

Steps:

1. Create an IAM user account(Administrative access).
2. AWS CLI configure:
   _1_. Fetch access keys and set aws CLI using these credentials `aws configure`

3. Create a new conda Env

# IAM ROle

Passing an IAM role gives Amazon SageMaker permission to perform actions in other AWS services on your behalf- services with in AWS necessary to perform required actions. We cant allocate permission to each one by one. so we use IAM ROLE

In `create notebook instance > Permission and Encryption`, if you select specific s3 bucket, it will have permission to access only that bucket.
