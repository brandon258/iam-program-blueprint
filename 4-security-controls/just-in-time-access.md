# Just-In-Time (JIT) Access Evaluation

## Overview

This document outlines my approach to evaluating Just-In-Time (JIT) access solutions for reducing privileged access exposure and accelerating access request turnaround times. JIT access improves security posture by granting elevated or sensitive access only when it is explicitly approved and needed—rather than relying on persistent permissions.

## Business Need

Many organizations struggle with prolonged access provisioning cycles, especially for elevated or time-sensitive permissions. This creates operational delays and increases the risk of over-provisioned accounts.

A JIT solution helps:

- Reduce standing access to sensitive systems
- Enable rapid, audit-ready approvals
- Improve compliance with HIPAA, SOC2, and internal controls

## Early Exploration Goals

In the early discovery phase, the goals were:

- Improve turnaround time from days/weeks → minutes
- Reduce friction for users needing temporary access
- Ensure approvals are auditable and time-bound
- Integrate with the existing IdP and HRIS

## Key Features

- **Time-boxed access** with automatic revocation
- **Approval workflows** with logging and notifications
- **Role-based JIT access** tied to just-in-time assignments
- **Audit trail** exportable to compliance systems
- **Integration** with existing tools (SSO, HRIS, ITSM)

## Potential Vendors

Initial vendors being considered include:

### 1. **Apono**

- SaaS-based JIT access and permissions manager
- Strong integrations with SaaS apps and cloud platforms
- Slack + Jira approval flows
- Agentless architecture

### 2. **Entitle (BeyondTrust-acquired)**

- Emphasizes enterprise access workflows
- Integrates with Okta, AWS, and on-prem
- Policy engine for justifications and usage tracking

### 3. **Okta JIT + Access Requests**

- Native to Okta platform
- Tightly coupled with Okta groups and policies
- Simpler deployment but limited to Okta-managed apps

## Considerations

| Factor            | Apono             | Entitle (BT)    | Okta Access Requests |
| ----------------- | ----------------- | --------------- | -------------------- |
| Cloud-native apps | ✅                | ✅              | ⚠️ (Okta only)       |
| Custom workflows  | ✅                | ✅              | ⚠️ Basic only        |
| On-prem support   | ❌ (cloud only)   | ✅              | ⚠️ Limited           |
| Cost/complexity   | ⚠️ (subscription) | ⚠️ (enterprise) | ✅ (native)          |
| Maturity          | Medium            | High            | Medium               |

## Next Steps

- Schedule vendor demos and security reviews
- Build a small proof-of-concept (POC) if needed
- Map existing roles and elevated access scenarios
- Ensure alignment with internal compliance and audit teams

## Summary

JIT access is a strategic control that reduces risk while improving agility. Several modern vendors offer compelling solutions, and the final choice will depend on:

- Integration needs
- Team workflows
- Long-term governance goals
