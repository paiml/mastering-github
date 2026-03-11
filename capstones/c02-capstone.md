# Capstone: Security, Identity, and Access

## Project Overview

A 50-person startup is moving from personal GitHub accounts to GitHub Enterprise Cloud. The CTO requires enforced 2FA, least-privilege repository access, and organization-wide security scanning before the migration is complete. Design and implement the full security architecture using a test organization and document every policy decision.

## Deliverables

### 1. Configure Authentication and Identity Controls

Create a GitHub organization and enforce 2FA for all members. Document the TOTP enrollment workflow, explain why TOTP is preferred over SMS, and describe the recovery code process for account lockout. Set up SSH key authentication for Git operations and create a scoped personal access token for API automation. Screenshot or describe each configuration step in the Security settings.

### 2. Design a Permission and Visibility Policy

Create three repositories with different visibility levels (public, private, internal if available) and document the risk implications of each. Establish a base permission level of read for the organization. Create at least two teams (e.g., "backend-engineers" and "contractors") and assign differentiated repository access — write for the engineering team, read for contractors. Produce a one-page policy document that maps each team role to a permission level (read, triage, write, maintain, admin) with justification grounded in least privilege.

### 3. Implement Organization Security Scanning and Collaborator Audit

Enable Dependabot alerts, code scanning, and secret scanning across all repositories from the organization Security tab. Invite a collaborator with triage-level access and document why triage was chosen over write. Review the Insights dashboard and summarize what the pull request, issue, and contributor metrics reveal about project health. Produce a brief access audit that lists every collaborator, their permission level, and whether that level is justified.

## Evaluation Criteria

### Distinction

- Enforces 2FA with TOTP, configures SSH keys and scoped API tokens, and articulates the authentication middleware layer where each credential type is verified
- Produces a policy cascade from organization base permissions through team grants to individual collaborator overrides, with each visibility and permission choice justified against specific threat scenarios (e.g., accidental secret exposure in public repos)
- Enables all three scanning types organization-wide, demonstrates the multi-repo coverage view, and connects Dependabot and secret scanning to supply-chain risk reduction with a concrete remediation workflow

### Proficient

- Configures 2FA and SSH keys correctly and assigns permission levels to teams with awareness of the member vs. owner role distinction
- Creates repositories at multiple visibility levels and documents the differences, but does not trace the full policy cascade from enterprise to organization to repository
- Enables security scanning and performs a collaborator audit, but does not connect scanning findings to organizational remediation processes

### Developing

- References 2FA, SSH, and permission levels but does not complete the enrollment workflow or explain the security rationale behind each configuration choice
- Creates repositories without varying visibility or assigning team-based permissions, resulting in all members having the same access
- Enables scanning features without reviewing results or auditing collaborator access levels
