# CCS6344 – Assignment 2  
## Secure Migration of a Traditional Application to AWS

**Author:** Muhammad Zarif Irfan Bin Suhaimi (241UC2414W)  
**GitHub:** [github.com/zrfifn](https://github.com/zrfifn)  
**Course:** CCS6344 – Database & Cloud Security, Multimedia University (MMU)
**Group:** Group 27
The Infrastructure as Code (IaC) templates and DevSecOps configuration for the secure migration of a traditional web application to the AWS cloud for CCS6344 Assignment 2.

The solution illustrates how an application can be migrated to a secure, multi-tier AWS architecture using Infrastructure as Code (CloudFormation) with a focus on cloud security best practices, including network segmentation, least-privilege IAM, encryption at rest and in transit, monitoring, logging, and web application protection.

A simple DevSecOps pipeline is also in place to automatically validate infrastructure security configurations.

## 📁 Repository Structure

```text
DBCS_A2_IAC/
├── 01-network.yml          # VPC, public & private subnets, routing
├── 02-security-groups.yml  # Security groups for ALB, App, and RDS
├── 03-rds-mysql.yml        # Encrypted RDS MySQL (Multi-AZ)
├── 04-app-alb.yml          # Application tier, ALB, EC2, IAM role
├── 05-s3-secure.yml        # Secure S3 bucket with encryption & public access block
├── 06-waf.yml              # AWS WAFv2 Web ACL with managed rules
├── buildspec.yml           # DevSecOps pipeline (cfn-lint security checks)
└── README.md
