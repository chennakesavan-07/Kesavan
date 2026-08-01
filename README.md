# AWS Application Load Balancer (ALB) Project

## Project Overview
This project demonstrates how to deploy a highly available web application using AWS.

## Services Used
- Amazon EC2
- Application Load Balancer (ALB)
- Amazon S3
- IAM Role
- Apache HTTP Server
- Security Groups

## Architecture
Internet
↓
Application Load Balancer
↙        ↘
EC2 Instance 1    EC2 Instance 2
↓
Amazon S3 (Images)

## Steps Performed
1. Created an IAM role with S3 read-only access.
2. Created an S3 bucket and uploaded images.
3. Launched two EC2 instances in different Availability Zones.
4. Installed Apache using EC2 User Data.
5. Created an Application Load Balancer.
6. Created a Target Group and registered both EC2 instances.
7. Verified that both targets were healthy.
8. Accessed the website using the ALB DNS name.

## Outcome
The Application Load Balancer successfully distributed traffic across two EC2 instances, providing a highly available web application.

## Screenshots
The repository contains screenshots of:
- EC2 Instances
- Application Load Balancer
- Target Group
- S3 Bucket
- Website accessed through the ALB DNS
