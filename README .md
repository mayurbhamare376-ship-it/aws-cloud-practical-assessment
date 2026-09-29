# AWS Cloud Practical Assessment

## Overview

This project demonstrates hands-on implementation of core AWS Cloud services with a focus on security, access management, compute, storage, database management, backup, and recovery.

## AWS Services Used

- AWS IAM
- Amazon EC2
- Amazon S3
- IAM Role
- Amazon RDS (MariaDB)
- Linux
- GitHub

---

# AWS Architecture Diagram

<p align="center">
  <img src="./aws-architecture-diagram.png" width="900">
</p>

---

# Q1 - IAM

IAM users, groups and permission policies were configured to demonstrate access control and permission management.

### Admin Access Denied

<p align="center">
  <img src="./Q1-IAM/adhar%20denied.png" width="800">
</p>

### ReadOnly Access Denied

<p align="center">
  <img src="./Q1-IAM/readonly-denied.png" width="800">
</p>

### S3 Access Denied

<p align="center">
  <img src="./Q1-IAM/s3%20denied.png" width="800">
</p>

---

# Q2 - EC2, S3 and IAM Role

An IAM Role was attached to the EC2 instance to provide secure access to Amazon S3 without configuring AWS access keys on the EC2 server.

### Admin Access

<p align="center">
  <img src="./Q2-EC2-S3-IAM-Role/Admin-access.png" width="800">
</p>

### AWS S3 Access

<p align="center">
  <img src="./Q2-EC2-S3-IAM-Role/AWS%20s3%20scr.png" width="800">
</p>

### IAM Role Test via SSH

<p align="center">
  <img src="./Q2-EC2-S3-IAM-Role/role%20test%20ssh.png" width="800">
</p>

---

# Q3 - RDS Backup and Recovery

An Amazon RDS MariaDB database was created and connected from the EC2 instance. Database data was created, a snapshot was taken, and the snapshot was used for recovery testing.

### RDS Connection

<p align="center">
  <img src="./Q3-RDS-Backup-Recovery/con%20MySQL.png" width="800">
</p>

### Students Database

<p align="center">
  <img src="./Q3-RDS-Backup-Recovery/Mysql%20students.png" width="800">
</p>

### Recovery Data Verification

<p align="center">
  <img src="./Q3-RDS-Backup-Recovery/Recovery%20data.png" width="800">
</p>

---

# Database Verification

```sql
SHOW DATABASES;
USE mayurdb;
SHOW TABLES;
SELECT * FROM students;
