# AWS EC2 Instance Deployment with GitHub Actions and Terraform

This project demonstrates how to use GitHub Actions to automatically deploy an EC2 instance on AWS using Terraform.

## Prerequisites

Before you begin, ensure you have the following:

1. **AWS Account**: Create an AWS account and set up an IAM user with the necessary permissions for creating EC2 instances.

2. **GitHub Repository**: Fork or clone this repository.

3. **GitHub Secrets**: In your repository settings, set up the following secrets:
   - `AWS_ACCESS_KEY_ID`: AWS IAM user access key.
   - `AWS_SECRET_ACCESS_KEY`: AWS IAM user secret key.

## Terraform Configuration
The `main.tf` file contains the Terraform configuration for the EC2 instance. Customize it based on your requirements.

## GitHub Actions Workflow
The .github/workflows/main.yml file defines the GitHub Actions workflow for deploying the EC2 instance.

## How to Use
Clone the repository: git clone https://github.com/pavankumarindian/aws-ec2-terraform-github-actions.git.

Set up AWS IAM user and obtain access key and secret key.

Add GitHub Secrets for AWS credentials.

Customize the main.tf file for your EC2 instance configuration.

Commit and push changes to the main branch.

Monitor the GitHub Actions workflow in the "Actions" tab.

## Cleanup
To avoid unnecessary AWS costs, remember to destroy the created resources. You can do this by updating the workflow to include a terraform destroy step.

## License
This project is licensed under the MIT License.
