# Home-Lab-Network

###### 

###### \# Day 0 - Project and Environment Setup:

* Created project repository and folder structure in GitHub.
* Created AWS root account using AWS Free Tier.
* Enabled root account MFA using Google Authenticator app on mobile.
* Set AWS Region as London (eu-west-2).



###### \# Day 1 - Billing and Foundations:

* AWS Billing and Cost Management - Created Zero-Spend Budget to notify if spending exceeds $0.00.
* AWS Billing and Cost Management - Created Monthly Cost Budget to notify if spending approaches or exceeds $5.00.



###### \# Day 2 - Identity and Access Management (IAM):

* AWS IAM - Created IAM user group 'Administrators', attaching the AdministratorAccess managed policy.
* AWS IAM - Created IAM user, and added them to Administrators user group.
* Logged in as IAM user, and will do so from now on unless root user account is needed.
* Verified access to EC2, IAM, S3, and Billing and Cost Management dashboards.



###### \# Day 3 - Building an Amazon VPC:

* VPCs - Created aws-lab-vpc, with IP address 10.0.0.0/16.
* Subnets - Created public-subnet-a within aws-lab-vpc, with IP address 10.0.1.0/24.
* Subnets - Enabled 'Auto-assign public IPv4 address' for public-subnet-a.
* Internet gateways - Created aws-lab-igw and attached it to aws-lab-vpc.
* Route tables - Created public route table and added 0.0.0.0/0 route to IGW.
* Route tables - Associated public-subnet-a with public-route-table.

