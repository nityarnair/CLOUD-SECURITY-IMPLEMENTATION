# CLOUD-SECURITY-IMPLEMENTATION

COMPANY : CODTECH IT SOLUTIONS

NAME : NITYA R NAIR

INTERN ID : CT04DK556

DOMAIN : CLOUD COMPUTING

DURATION : 4 WEEKS

MENTOR : NEELA SANTOSH

#DESCRIPTION :
For Task 4 of my internship, I was asked to implement cloud security practices using **Amazon Web Services (AWS)**. The main objective was to understand how to manage user access, securely store data, and ensure that stored data is protected through encryption. This hands-on task helped me understand basic cloud security concepts in a real AWS environment.

Since I already had an AWS account, I began by setting up **IAM (Identity and Access Management)** to control access. Using the IAM console, I created a new user specifically for this task (separate from the root user, which should only be used for critical account-level actions). I gave the new user both **console access** and **programmatic access** and assigned two policies: `AmazonS3FullAccess` for storage-related permissions and `IAMReadOnlyAccess` to allow viewing of IAM configurations without being able to modify them. To improve security, I also enabled **MFA (Multi-Factor Authentication)** on the user account. This added an extra step to the login process, using an app like Google Authenticator.

Next, I moved on to configuring **S3 (Simple Storage Service)**, AWS’s storage solution. I created a new S3 bucket, gave it a unique name, and selected the region closest to me for better performance. I left public access blocked (which is recommended for security), and I enabled **versioning**. Versioning helps keep track of changes to files and allows you to restore previous versions if something is accidentally deleted or overwritten.

I uploaded a test file to the bucket to confirm that everything was working correctly. Once the bucket was ready, I configured **encryption**. I used **SSE-S3 (Server-Side Encryption with S3-managed keys)** to encrypt objects at rest automatically. This ensures that even if someone could access the data storage layer, they wouldn’t be able to read the contents without decryption. I also noted that AWS uses HTTPS by default for all S3 interactions, so data is encrypted **in transit** as well.

As an optional step, I enabled **AWS CloudTrail**, which tracks all actions taken in the AWS account. I created a new trail to log all management events and stored the logs in the same S3 bucket. This helps monitor account activity, detect unusual behavior, and maintain an audit trail.

To complete the task, I documented each step with relevant screenshots and created a final report summarizing what I did. The report included the IAM setup, S3 configurations, encryption settings, and CloudTrail monitoring.

##OUTPUT :
