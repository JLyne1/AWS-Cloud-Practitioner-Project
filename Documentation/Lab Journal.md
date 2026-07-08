# Home-Lab-Network

###### 

###### \# Day 0 - Project and Environment Setup:

* Created project repository and folder structure in GitHub.
* Created AWS root account using AWS Free Tier.
* Enabled root account MFA using Google Authenticator app on mobile.
* Set AWS Region as London (eu-west-2).



###### \# Day 1 - Billing and Foundations:

* Billing and Cost Management - Created Zero-Spend Budget to notify if spending exceeds $0.00.
* Billing and Cost Management - Created Monthly Cost Budget to notify if spending approaches or exceeds $5.00.



###### \# Day 2 - Identity and Access Management (IAM):

* IAM - Created IAM user group 'Administrators', attaching the AdministratorAccess managed policy.
* IAM - Created IAM user, and added them to Administrators user group.
* Logged in as IAM user, and will do so from now on unless root user account is needed.
* Verified access to EC2, IAM, S3, and Billing and Cost Management dashboards.



###### \# Day 3 - Building an Amazon VPC:

* VPCs - Created aws-lab-vpc, with IP address 10.0.0.0/16.
* Subnets - Created public-subnet-a within aws-lab-vpc, with IP address 10.0.1.0/24.
* Subnets - Enabled 'Auto-assign public IPv4 address' for public-subnet-a.
* Internet gateways - Created aws-lab-igw and attached it to aws-lab-vpc.
* Route tables - Created public route table and added 0.0.0.0/0 route to IGW.
* Route tables - Associated public-subnet-a with public-route-table.



###### \# Day 4 - Launching an Amazon EC2 Instance:

* Key Pairs - Created aws-lab-key.pem, and stored it outside of Git repository.
* Instances - Created instance aws-lab-web-server, using Amazon Linux 2023 AMI and t3.micro instance type.
* Instances - Created security group aws-lab-web-sg.
* Instances - Successfully launched aws-lab-web-server.
* Windows PowerShell unable to establish SSH connection with aws-lab-web-server - See Day 4/Issue 1 in Troubleshooting.
* Used SSH within Windows PowerShell to connect to aws-lab-web-server.
* Web server hostname confirmed as ip-10-0-1-54.eu-west-2.compute.internal.
* Pings were unsuccessful, but curl commands performed as expected.

