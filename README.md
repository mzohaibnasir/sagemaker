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

In `create notebook instance > Permission and Encryption`, if you select specific s3 bucket, it will have permission to access only that bucket. With `any bucket`, this application will access all buckets.

# class S3.Object(bucket_name, key)

A resource representing an Amazon Simple Storage Service (S3) Object:
"""
import boto3

s3 = boto3.resource('s3')
object = s3.Object('bucket_name','key')

"""

# Estimator

The sagemaker.estimator.Estimator is a high-level interface for SageMaker training in the Amazon SageMaker Python SDK. It is used to create and manage training jobs, as well as to deploy trained models. The Estimator class allows you to specify the training image URI, role, instance type, instance count, output path, and other parameters to create a training job. Once the training job is created, you can call the fit method to start the training process. After the training is complete, you can deploy the trained model using the deploy method
