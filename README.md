# Lift-shift-application-wworkload
Architecture of AWS Services for the project : EC2 instance, ELB, Autoscaling, EFS/S3 for storage, Amazon Certificate manage, Route53.

Multi-tier Web Application stack, which is hosts and run on AWS cloud for production using Lift and Shift strategy.

FLOW OF EXECUTION:

Login to AWS Account
Create Key Pairs
Create Security groups
Launch Instances with user data [BASH SCRIPTS]
Update IP to name mapping in route 53
Build Application from source code
Upload to S3 bucket
Download artifact to Tomcat Ec2 Instance
Setup ELB with HTTPS [Cert from Amazon Certificate Manager]
Map ELB Endpoint to website name in Godaddy DNS
Verify
Build Autoscaling Group for Tomcat Instances.
