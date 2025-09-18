# Access Review Automation Example

This section describes a real-world IAM automation project I helped design and implement to support quarterly access reviews and compliance with HIPAA and SOC2.

## Problem

Certain cloud applications were not fully integrated with our primary IdP, making it difficult to perform accurate quarterly access reviews. Manual reviews were time-consuming and error-prone.

## Solution

We built a lightweight automation tool in AWS that performs cross-referencing between our source of truth for active employees and each application's user base via API.

## Key Features

- **Runs on AWS Lambda** with supporting infrastructure via IaC
- **Pulls active employee data** from internal directory using the REST API
- **Fetches user lists** from applications using their public APIs
- **Compares users** and flags accounts that exist in the app but not in directory
- **Generates reports** in `.xlsx` format and stores them in S3 for auditing
- **Notifies stakeholders** via email and/or Jira ticket when discrepancies are found

## Compliance Impact

- Supports **SOC2 and HIPAA quarterly access review controls**
- Creates durable evidence for auditors
- Reduced manual effort and review cycle time

## Tools & Technologies

- AWS Lambda (Python)
- Directory REST API
- Application APIs
- AWS S3 for output storage
- IAM roles for secure access
- GitHub Actions for CI/CD

## Outcome

- Improved review accuracy
- Reduced review time from hours to minutes
- Increased visibility into orphaned accounts
