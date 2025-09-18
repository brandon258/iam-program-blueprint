# IAM Program Blueprint

## Overview

This repository provides a strategic and technical blueprint for building an Identity & Access Management (IAM) program from scratch in a modern enterprise environment.

While I have not yet led a greenfield IAM initiative professionally, this project showcases how I would approach the challenge—both at a high level and with tangible artifacts, templates, and working code. It is intended to demonstrate readiness for roles that require end-to-end IAM leadership.

---

## Repository Structure

```
iam-program-blueprint/
├── README.md
├── 0-strategy/
│ ├── iam-vision.md
│ ├── stakeholder-map.md
│ └── governance-model.md
├── 1-discovery/
│ ├── systems-inventory-template.xlsx
│ ├── identity-data-flow-diagram.png
│ └── questions-for-stakeholders.md
├── 2-architecture/
│ ├── high-level-architecture.drawio
│ ├── idp-vs-sp-decision.md
│ └── identity-lifecycle.md
├── 3-implementation/
│ ├── open-source-vs-commercial.md
│ ├── example-poc/
│ │ ├── README.md
│ │ ├── docker-compose.yml
│ │ └── keycloak-fastapi-poc/
├── 4-security-controls/
│ ├── mfa-policy.md
│ ├── least-privilege-principles.md
│ ├── secrets-management.md
│ └── just-in-time-access.md
├── 5-governance-and-operations/
│ ├── access-review-process.md
│ ├── access-review-automation.md
│ ├── onboarding-offboarding.md
│ └── break-glass-access.md
└── 6-future-considerations/
├── passwordless.md
├── identity-governance.md
└── audit-readiness.md
```

---

## Project Goals

- Show how I would design and scale an IAM program from scratch.
- Provide practical code and architecture examples.
- Include strategy, security, and governance best practices.
- Demonstrate tools I’ve worked with (Keycloak, Auth0, Terraform, Okta, AWS IAM, etc.).
- Communicate systems thinking, leadership, and security expertise.

---

## IAM Program Pillars

### 1. Strategy & Vision

- IAM should enable productivity securely—not create friction.
- Design for automation, auditability, and scalability.
- Balance security and usability.

### 2. Discovery & Stakeholder Engagement

- Start with systems inventory and stakeholder interviews.
- Understand existing access patterns and pain points.
- Diagram identity data flows from HRIS to endpoints.

### 3. Architecture & Integration

- Choose IdP (Okta, Keycloak, Auth0) based on ecosystem.
- Design SSO patterns (SAML/OIDC) with just-in-time provisioning.
- Implement SCIM, RBAC/ABAC, and access workflows.
- Integrate with AWS, Kubernetes, and CI/CD systems.

### 4. Security Controls

- Enforce MFA with adaptive and FIDO2 support.
- Enforce least privilege with role modeling.
- Use Terraform or GitOps to manage identity infrastructure.

### 5. Governance & Operations

- Define joiner/mover/leaver flows.
- Automate access reviews and role cleanup.
- Centralize logging and audit trails for review and incident response.

### 6. Future Considerations

- Move toward passwordless and passkeys.
- Introduce IGA platforms as needed (SailPoint, Saviynt).
- Maintain security posture through continuous access analytics.

---

## IAM Projects Included

- [Access Review Process](./5-governance-and-operations/access-review-process.md)
- [Access Review Automation](./5-governance-and-operations/access-review-automation.md)
- [Just-in-Time Access Evaluation](./4-security-controls/just-in-time-access.md)

---

## Tech Stack & Tooling

- **Languages**: Python, Bash, HCL (Terraform)
- **IAM Tools**: Keycloak, Okta, Azure Entra ID, AWS IAM
- **Protocols**: OAuth 2.0, OpenID Connect, SAML, SCIM, FIDO2
- **Infrastructure**: AWS, Kubernetes (EKS), Docker, GitHub Actions

---

## About the Author

This repo is maintained by an engineer focused on Identity, DevOps, and platform security. It serves both as a learning aid and a demonstration of how I approach end-to-end IAM ownership in a modern cloud-native enterprise.

You can view more of my work or connect with me on [LinkedIn](https://www.linkedin.com/in/brandonhelmer/).

---

## Status

Initial structure is complete. Artifacts and diagrams coming soon.

---

## License

MIT License
