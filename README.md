# Three-tier AWS Architecture

The three-tier architecture template includes:

- Web tier with:
-- Public subnets
-- Auto Scaling Group with EC2 instances
-- Internet-facing Application Load Balancer
- Application tier with:
-- Private subnets
-- Auto Scaling Group with EC2 instances
-- Internal Application Load Balancer
- Database tier with:
-- Private subnets
-- Multi-AZ SQL Server 2022 RDS instance
-- Proper security isolation

The template follows AWS best practices with proper network segmentation, security groups, and high availability configurations. You can now use this template to deploy your three-tier architecture in the ap-southeast-1 region.
