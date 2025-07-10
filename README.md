# Provisioning an AWS EC2 Instance using Terraform

This project demonstrates how to use Terraform to automate the provisioning of an EC2 instance on AWS. It is designed for beginners to understand the basics of Infrastructure as Code (IaC), Terraform syntax, and AWS resource deployment.

## Prerequisites

Ensure you have the following tools installed:

- Terraform
- AWS CLI
- Visual Studio Code
- VSCode Extensions:
  - AWS Toolkit
  - Terraform
  - Remote - SSH

AWS IAM User Setup (Terraform)

To allow Terraform to interact with AWS services securely, you'll need to create an IAM user with programmatic access.

1. Go to the IAM Console `https://console.aws.amazon.com/iam`

2. Create a New User by navigating to Users > Create users

Enter a username (e.g., terraform-user)

Leave Console access unchecked (unless console access is also needed)

Click Next

3.  Attach policies directly `AdministratorAccess`

4. Skip Groups, Tags, and Permissions boundary

5. Click Create user

6. Generate Programmatic Access
After user creation:

Click the newly created user from the list

Go to the Security credentials tab

Scroll to Access keys section

Click “Create access key”

Choose “Application running outside AWS”

Click Next, then Create access key

✅ Download the .csv file containing:

Access Key ID

Secret Access Key

⚠️ Important: Keep this .csv file safe. Do not share or upload it publicly.