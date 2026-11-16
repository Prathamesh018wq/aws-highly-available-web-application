# Highly Available Web Application on AWS

## Project Overview
Designed and implemented a highly available web application infrastructure on AWS using core cloud and DevOps services.

## AWS Services Used
- Amazon VPC – Network isolation
- Amazon EC2 – Web server hosting
- Application Load Balancer – Traffic distribution
- Auto Scaling Group – Instance scaling
- Amazon RDS (MySQL) – Database
- Amazon S3 – Database backup storage
- AWS IAM – Access management
- Amazon CloudWatch – Monitoring and alarms
- Amazon SNS – Email notifications

## Key Implementations
- Created VPC with two public subnets across Availability Zones.
- Configured EC2 and Nginx web server.
- Configured Application Load Balancer and Target Group.
- Created Launch Template and Auto Scaling Group.
- Connected EC2 to RDS MySQL.
- Configured IAM role for secure S3 access.
- Automated database backups using a shell script and cron.
- Uploaded compressed database backups to S3.
- Performed database restore testing successfully.
- Configured CloudWatch alarms and SNS email alerts.
- Created a CloudWatch monitoring dashboard.

## Backup and Disaster Recovery
- Automated MySQL database backup using `mysqldump`.
- Stored compressed backups in Amazon S3.
- Restored backup into a separate test database.
- Verified all three employee records after restore.

## Monitoring
- CPU Utilization monitoring
- EC2 Status Check monitoring
- High CPU alarm threshold: 70%
- Status Check failure alarm threshold: 1
- SNS email notification tested successfully

## Important Note
This is a hands-on learning and portfolio project, not a production deployment. The database subnet design uses public subnets; production environments should use private database subnets and additional security controls.

## Author
GitHub: https://github.com/Prathamesh018wq

