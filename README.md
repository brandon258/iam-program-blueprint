# IAM Program Blueprint

## Overview

This repository provides a strategic and technical blueprint for building an Identity & Access Management (IAM) program from scratch in a modern enterprise environment.

While I have not yet led a greenfield IAM initiative professionally, this project showcases how I would approach the challenge—both at a high level and with tangible artifacts, templates, and working code. It is intended to demonstrate readiness for roles that require end-to-end IAM leadership, such as the Senior IAM Engineer role at Moveworks.

---

## Repository Structure

```
iam-program-blueprint/
├── README.md
├── 0-strategy/
│   ├── iam-vision.md
│   ├── stakeholder-map.md
│   └── governance-model.md
├── 1-discovery/
│   ├── systems-inventory-template.xlsx
│   ├── identity-data-flow-diagram.png
│   └── questions-for-stakeholders.md
├── 2-architecture/
│   ├── high-level-architecture.drawio
│   ├── idp-vs-sp-decision.md
│   └── identity-lifecycle.md
├── 3-implementation/
│   ├── open-source-vs-commercial.md
│   ├── example-poc/
│   │   ├── README.md
│   │   ├── docker-compose.yml
│   │   └── keycloak-fastapi-poc/
├── 4-security-controls/
│   ├── mfa-policy.md
│   ├── least-privilege-principles.md
│   └── secrets-management.md
├── 5-governance-and-operations/
│   ├── access-review-process.md
│   ├── onboarding-offboarding.md
│   └── break-glass-access.md
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
- Demonstrate tools I’ve worked with (Keycloak, FastAPI, Terraform, Okta, AWS IAM, etc.).
- Communicate systems thinking, leadership, and security expertise.

---

## Tech Stack & Tooling

- **Languages**: Python, Bash, HCL (Terraform)
- **IAM Tools**: Keycloak, Okta, Azure Entra ID, AWS IAM
- **Protocols**: OAuth 2.0, OpenID Connect, SAML, SCIM, FIDO2
- **Infrastructure**: AWS, Kubernetes (EKS), Docker, GitHub Actions

---

## Status

🚧 Initial scaffolding in progress — contributions to each folder coming soon.

---

## License

MIT License
