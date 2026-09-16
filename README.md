# AWS Auto Scaling with Mixed Instances & Chaos Testing

## Overview

This project demonstrates a highly available and resilient AWS application infrastructure using:

- Application Load Balancer (ALB)
- EC2 Auto Scaling Group
- Mixed Instances Policy
- On-Demand Instances
- Spot Instances
- Launch Template
- Lifecycle Hooks
- Instance Warm-up
- CloudWatch
- Automatic Scaling
- Chaos Testing

## Architecture

User
  |
  v
Application Load Balancer
  |
  v
Target Group
  |
  v
Auto Scaling Group
  |
  +----------------------+
  |                      |
  v                      v
On-Demand EC2        Spot EC2
  |                      |
  +----------+-----------+
             |
             v
        CloudWatch

## Key Features

- Mixed On-Demand and Spot EC2 capacity
- Automatic scaling based on CPU utilization
- ALB request-count based scaling
- Lifecycle hook for instance initialization
- Instance warm-up before production traffic
- Automatic replacement of unhealthy instances
- Instance termination chaos testing
- Availability Zone resilience testing
- CloudWatch monitoring

## Technologies

- AWS EC2
- AWS Auto Scaling
- AWS Application Load Balancer
- AWS Target Groups
- AWS CloudWatch
- AWS IAM
- AWS VPC
- Amazon Linux

## Project Goals

1. Build a highly available EC2 infrastructure.
2. Reduce compute cost using Spot Instances.
3. Maintain reliability using On-Demand capacity.
4. Automatically scale based on application load.
5. Test application resilience through controlled failures.
6. Demonstrate AWS DevOps and cloud infrastructure skills.

## Testing

The project includes:

- EC2 instance termination testing
- Auto Scaling replacement testing
- Availability Zone failure simulation
- Load-based scaling testing
- Lifecycle hook validation
- Spot interruption resilience testing

## Author

Aarchi Patel
