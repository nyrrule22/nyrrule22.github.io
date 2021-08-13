---
layout: page
title: Beginners Guide to IAM
permalink: /notes/aws/aws_certified_developer-associate/bgtiam
tags: aws
---
# Beginners Guid to IAM

# IAM 101
## IAM Basics
### What does IAM Provide?
- Centralized: Control of your AWS account
- Access: Shared access to your AWS account
- Permissions: Granular permissions
- Identity Federation: Supports well-known identity providers such as: AD, Facebook, and LinkedIn
### IAM
- Multi-Factor Authentication: Provides increases security for your AWS account settings and resources
- Temporary Access: Provides temporary access for users/devices and services, as necessary
- Password Policies: Allows you to set up your own password rotation policy
- Integrated: Integrates with many different AWS services.
- Compliance: Supports PCI DSS compliance
### Core Concepts
- Users: End users - think people
- Groups: A collection of users under one set of permissions
- Roles: You create roles and can then assign them to users, applications, and - services to give access to AWS resources
### IAM Policy
- A document that defines one or more permissions
- An IAM policy can be attached to a user, group, or role
# Testing IAM Policy Permissions
## IAM Policy Simulator
- Test the effects of IAM policies before committing them to production
- Validate that the policy works as expected
- Test policies already attached to existing users - great for troubleshooting an issue which you suspect is IAM related
- https://policysim.aws.amazon.com
# IAM 101 Summary
- IAM is universal, not regional
- The root account is created when you first set up your AWS account. The account has complete admin access.
- New users have no permissions when first created
### IAM Access Keys - Exam Tips
- Access Keys: New Users are assigned an access key ID and secret access key when their accounts are created
- Not for Console Access: These are not the same as a password, and you cannot use the access key ID or secret access key to log into the AWS Management Console.
- Programmatic Access: You can use access keys to access AWS via the APIs and command line
- Viewing Access Keys; You only get to view the access key ID and secret access key once. If you lose them, you have to regenerate them. Make sure to save them in a secure location.
- Use MFA: Always set up Multi-Factor Authentication (MFA) on your root account.
- Password Rotation: You can create and customize your own password rotation policies.

###### tags: `aws`
