# Heyy there I am Mohammed Thalib,

#  Here you will find my project that I had worked and gained hands on experience in Devops.
    
#                                                                         DevOps-Project-1
#                                                            Deploy Java Application on AWS Architecture

![AWS Architecture](https://imgur.com/b9iHwVc.png)

## Table of Contents

1. [Project Overview](#project-overview)
2. [Architecture Overview](#architecture-overview)

   ## Introduction

This project demonstrates the deployment of a production-grade Java web application using AWS's robust architecture. The implementation follows cloud-native best practices, ensuring high availability, scalability, and security across all application tiers.

### Key Features

- **High Availability**: Multi-AZ deployment with automated failover
- **Auto Scaling**: Dynamic resource allocation based on demand
- **Security**: Defense-in-depth approach with multiple security layers
- **Monitoring**: Comprehensive logging and monitoring setup
- **Cost Optimization**: Efficient resource utilization and management

## Architecture Overview

### Infrastructure Components

1. **Presentation Tier (Frontend)**
   - Nginx web servers in Auto Scaling Group
   - Public-facing Network Load Balancer
   - CloudFront Distribution for static content

2. **Application Tier (Backend)**
   - Apache Tomcat servers in Auto Scaling Group
   - Internal Network Load Balancer
   - Session management with Amazon ElastiCache

### Network Architecture

- **VPC Design**
  - Two separate VPCs (192.168.0.0/16 and 172.32.0.0/16)
  - Public and private subnets across multiple AZs
  - Transit Gateway for inter-VPC communication
