# AWS CI Pipeline for Infrastructure Security

This project demonstrates how real-world companies validate AWS infrastructure
code using AWS-native CI pipelines before deployment.

## What this project shows
- Infrastructure as Code using CloudFormation
- AWS CodePipeline + CodeBuild for CI
- Security and syntax validation using cfn-lint
- GitHub as source, AWS as execution environment

## How it works
1. Developer pushes infrastructure code to GitHub
2. GitHub webhook triggers AWS CodePipeline
3. CodeBuild runs validation checks inside AWS
4. Build fails if security or syntax issues are found

## Why this matters
In production environments, developers do not deploy infrastructure directly.
All changes must pass AWS-controlled CI checks for security, compliance,
and auditability.

## Tools used
- AWS CodePipeline
- AWS CodeBuild
- AWS CloudFormation
- cfn-lint
- GitHub
