# Questions for IAM Stakeholder Discovery

These are the first questions I would ask key stakeholders (Security, IT, HR, Engineering, Compliance) when baselining an IAM program.

## 1. Business & Security Objectives

- What are your top identity-related risks or pain points?
- Are there any regulatory or compliance requirements (e.g., HIPAA, SOC 2, FedRAMP)?

## 2. User Lifecycle

- How are new users onboarded today? Who approves access?
- What systems are involved in offboarding?
- Are contractors handled differently?

## 3. Access Patterns

- What are the most sensitive systems and who has access to them?
- How is temporary or elevated access currently granted?

## 4. Tooling & Integration

- What IdP is currently used (if any)? SSO? SCIM?
- Are cloud platforms (AWS, GCP, Azure) tied into the identity system?

## 5. Audit & Monitoring

- How are access reviews currently performed?
- Are authentication logs ingested into a SIEM or alerting tool?
