AWS IAM (Identity and Access Management)
-----------------------------------------

AWS Identity and Access Management (IAM) is a service that helps you securely manage access to AWS resources. 

It enables you to control who can access your AWS account, what they can do, and which resources they can use.

### Key Concepts of AWS IAM

1. IAM Users
A user represents a person or an application that interacts with AWS.
Each user has unique credentials (username and password or access keys).
Users can be assigned permissions to access specific AWS services.
2. IAM Groups
A group is a collection of IAM users.
Instead of assigning permissions to individual users, you assign permissions to a group, and all users in that group inherit those permissions.
Example: A Developers group may have access to EC2, while a Data Engineers group may have access to S3 and Redshift.
3. IAM Roles
An IAM role is not tied to a specific user but can be assumed by AWS services or users.
Used when AWS services (like Lambda, EC2, or Glue) need permissions to access other AWS resources.
Example: An EC2 instance role allows an EC2 instance to access S3 without using access keys.
4. IAM Policies
Policies define what actions are allowed or denied for a user, group, or role.

Policies are written in JSON format and specify:

Effect: Allow or Deny
Actions: The AWS service and operations (e.g., s3:PutObject)
Resources: The AWS resources affected (e.g., arn:aws:s3:::my-bucket/*)
Types of Policies:

Managed Policies: Predefined policies by AWS (e.g., AdministratorAccess, AmazonS3ReadOnlyAccess).
Customer Managed Policies: Custom policies created by users.
Inline Policies: Policies embedded directly in a user, group, or role.

5. IAM Access Control Mechanisms
Least Privilege Principle: Grant only the permissions needed to perform a task.
MFA (Multi-Factor Authentication): Adds an extra layer of security by requiring a second authentication method.
IAM Access Analyzer: Helps review permissions and identify overly permissive access.
AWS Organizations: Manages IAM policies across multiple AWS accounts.
Best Practices for Using AWS IAM
Follow the Principle of Least Privilege – Grant only the permissions needed.
Enable MFA for all IAM Users – Adds an extra security layer.
Use IAM Roles Instead of Access Keys – Avoid storing long-term access keys.
Regularly Review IAM Policies – Remove unnecessary permissions.
Use AWS Organizations & SCPs – Manage access across multiple AWS accounts.
Monitor IAM Activity with AWS CloudTrail – Tracks API calls and changes to IAM users, roles, and policies.
