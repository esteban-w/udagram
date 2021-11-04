# Infrastructure Description

In order for this project to successfully be built and deployed, the following resources are needed:
- AWS RDS database running Postgres 
  - Version PostgreSQL 12.5-R1
  - Initial DB instance size: db.t2.micro
  - Connectivity: Public access YES
- AWS Elastic Beanstalk
  - Web server environment
  - Platform: NodeJS 12 running on 64bit Amazon Linux 2
- AWS S3 bucket for server media files
  - All Public access enabled
  - Bucket policy with write and get permissions
  - CORS enabled
- AWS S3 bucket for hosting Frontend application
  - All Public access enabled
  - Bucket policy with get permissions
  - Static website hosting enabled
- Circle CI for creating a basic pipeline and connected to project's repository  