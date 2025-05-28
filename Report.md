**REPORT**

1. IAM Configuration

Created user: intern-user

Attached policies: AmazonS3FullAccess, IAMReadOnlyAccess

Enabled MFA

2. Secure Storage
   
Created bucket: internbucketnitya

Enabled versioning

Uploaded file: image.jpg

Blocked public access: Yes

3. Encryption
   
Used: SSE-S3 encryption at rest

HTTPS used: Yes (default for S3)

4. Monitoring
   
Created CloudTrail to log all events

Logs stored in same S3 bucket
