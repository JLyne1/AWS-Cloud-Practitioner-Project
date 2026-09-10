### AWS Security Review



##### Security and Compliance

* Identity and Access

  * IAM
  * IAM Roles



* Network Security

  * Security Groups
  * Network ACLs



* Data Protection

  * S3 encryption (SSE-S3)
  * KMS



* Monitoring and Detection

  * CloudWatch
  * CloudTrail



* Recommendations

  * Trusted Advisor



* Compliance

  * AWS Artifact





##### Account Security

* Root account MFA: Enabled
* Root account access keys: Not configured
* IAM user MFA: Enabled
* IAM user used for normal administration: Yes



* IAM

  * Administrators group configured
  * Current user has administrative permissions
  * Least privilege review: Required for production use



* EC2

  * Security Group: aws-lab-web-sg
  * Inbound:

    * SSH / TCP 22 / My IP
    * HTTP / TCP 80 / 0.0.0.0/0



* S3

  * Block Public Access: Enabled
  * Object Ownership: Bucket owner enforced
  * Versioning: Enabled
  * Server-side encryption: Enabled



* Monitoring

  * CloudWatch: Configured
  * CloudTrail: Reviewed
  * Trusted Advisor: Reviewed



* Security Model

  * AWS is responsible for security of the underlying cloud infrastructure.
  * The customer is responsible for security configuration and data within the cloud, according to the service being used.

