# AWS

This tutorial will guide you through the process of using the AWS terminal to manage your cloud resources.

## Prerequisites

Before starting this tutorial, ensure that you have the following:

- An AWS account
- AWS CLI installed on your machine
- Basic knowledge of AWS services

## Steps

1. Open your terminal and enter the command `aws configure`. This will prompt you to enter your Access key ID, Secret access key, Default region name, and Default output format.
2. After entering the required details, you can now start using the AWS CLI to manage your resources.
3. To list all your AWS S3 buckets, enter the command `aws s3 ls`.
4. To create a new S3 bucket, enter the command `aws s3 mb s3://bucket-name`. Replace `bucket-name` with the name you want to give your bucket.
5. To delete an S3 bucket, enter the command `aws s3 rb s3://bucket-name --force`.
6. To list all your EC2 instances, enter the command `aws ec2 describe-instances`.
7. To start an EC2 instance, enter the command `aws ec2 start-instances --instance-ids instance-id`. Replace `instance-id` with the ID of the instance you want to start.
8. To stop an EC2 instance, enter the command `aws ec2 stop-instances --instance-ids instance-id`. Replace `instance-id` with the ID of the instance you want to stop.

## [[staging]]

```shell
sudo su centos 
cd /var/www/vhosts/staging."enviroment"/"enviroment"
```

## [[uat]]

```shell
sudo su centos 
cd /var/www/vhosts/uat."enviroment"/"enviroment"
```

## [[Scripts]]

```shell
./scripts/run-jobs.sh
```