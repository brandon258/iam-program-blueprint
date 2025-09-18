# Access Review Process (Sample)

## Review Cadence

- Quarterly access reviews for critical systems (e.g., prod, financial systems)
- Semi-annual reviews for internal/low-risk systems

## Review Owners

- System Owners validate each user's access
- Reviewers receive export files via email or Jira ticket

## Automation

- User list pulled from HR system (e.g., BambooHR)
- Cross-referenced with app-level users (Bitbucket, Imperva, etc.)
- Lambda function outputs a .xlsx report to S3 with unmatched accounts flagged

## Sample Controls

- Flag accounts not linked to active employees
- Alert on shared accounts or missing owner metadata
- Time-boxed temporary access (e.g., 30-day expiration)

## Audit

- Signed reviews stored in S3 with versioning enabled
- Reports attached to Jira for traceability
