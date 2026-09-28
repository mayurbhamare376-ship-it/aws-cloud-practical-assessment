# AWS Cloud Practical Assessment

## Overview
This project demonstrates practical AWS Cloud concepts including IAM, EC2, S3, IAM Roles, Amazon RDS, backup and database recovery.

## AWS Services Used
- IAM
- EC2
- S3
- IAM Role
- Amazon RDS
- MySQL
- Linux

## Project Structure

- Q1-IAM
- Q2-EC2-S3-IAM-Role
- Q3-RDS-Backup-Recovery

## Q1 - IAM
Configured IAM users, permissions and access management.

## Q2 - EC2, S3 and IAM Role
Created an EC2 instance and configured access to AWS resources using an IAM Role.

## Q3 - RDS Backup and Recovery
Created an Amazon RDS MySQL database, configured security settings, created backup/snapshot and verified database recovery.
## Q3 - RDS Backup and Recovery

### RDS Database Created
![RDS Created](./Q3-RDS-Backup-Recovery/rds-created.png)

### RDS Database Available
![RDS Available](./Q3-RDS-Backup-Recovery/rds-available.png)

### Security Group Configuration
![RDS Security Group](./Q3-RDS-Backup-Recovery/rds-security-group.png)

### RDS Endpoint
![RDS Endpoint](./Q3-RDS-Backup-Recovery/rds-endpoint.png)

### Database Recovery Verification
![Data Verification](./Q3-RDS-Backup-Recovery/rds-data-verification.png)

## Database Verification

Database status was verified after recovery using MySQL commands.

```sql
SHOW DATABASES;
SHOW TABLES;
SELECT * FROM students;