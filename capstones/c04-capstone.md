# Capstone: Enterprise Administration Across Seven Domains

## Project Overview

A 200-person fintech company is migrating from GitHub Team to GitHub Enterprise Cloud. The VP of Engineering requires centralized identity management with SAML SSO, enforced security policies across all 40 repositories, a self-hosted runner infrastructure for CI/CD, and a GitHub Packages registry for internal libraries. Design and implement the full enterprise administration architecture across all seven domains using a test enterprise account.

## Deliverables

### 1. Configure Enterprise Identity and Access Management

Set up SAML SSO at the enterprise level and document the IdP integration workflow including attribute mapping for user provisioning. Configure Enterprise Managed Users with SCIM provisioning and explain when EMU accounts are preferred over personal accounts with SSO. Enforce two-factor authentication across all organizations and establish a tiered permission model — map the principle of least privilege from enterprise owner down through organization owner, team maintainer, and repository-level roles. Produce a permission matrix that documents every role, its scope, and the justification for each access grant.

### 2. Implement Security Compliance and Repository Governance

Enable Dependabot alerts, code scanning, and secret scanning at the enterprise level so all current and future repositories inherit the policy. Configure repository visibility rules — set a default of internal visibility and document the approval process for public repositories. Create a security audit that reviews three representative repositories: list all collaborators, their permission levels, enabled scanning features, and any policy violations. Demonstrate the enterprise audit log by querying for authentication events and permission changes over the past 30 days.

### 3. Deploy GitHub Actions at Scale with Package Registry

Configure a runner group with self-hosted runners scoped to the production organization and document the security boundary between runner groups. Create a reusable workflow that runs linting, testing, and deployment steps, then call it from three different repositories using `workflow_call`. Set up the GitHub Packages container registry (ghcr.io) and publish a Docker image using GITHUB_TOKEN authentication in a workflow. Document the difference between GitHub Packages and GitHub Releases, and explain when each distribution mechanism is appropriate for the company's internal libraries versus public SDKs.

## Evaluation Criteria

### Distinction

- Configures SAML SSO with EMU provisioning and produces a permission matrix tracing the principle of least privilege from enterprise through organization to repository level, with each grant justified against a specific threat scenario
- Enables all security scanning features enterprise-wide with inheritance verification, demonstrates the audit log with targeted queries, and connects scanning findings to a remediation workflow with SLA commitments
- Deploys scoped runner groups with documented security boundaries, implements reusable workflows called across repositories, and publishes packages to ghcr.io with a clear distribution strategy distinguishing Packages from Releases

### Proficient

- Configures SSO and 2FA enforcement with correct role assignments across organizations and teams, but does not trace the full permission cascade from enterprise to repository or justify each access decision
- Enables security scanning and performs a collaborator audit, but does not demonstrate audit log queries or connect findings to a remediation process
- Creates working Actions workflows and publishes a package, but does not use reusable workflows or document runner group security boundaries

### Developing

- References SSO, EMU, and permission levels but does not complete the IdP integration or produce a permission matrix
- Enables scanning features without reviewing results across repositories or auditing collaborator access
- Creates a workflow that runs but does not demonstrate enterprise-scale patterns like reusable workflows, runner groups, or package publishing

## Share Your Work

Add this capstone to your LinkedIn profile as a portfolio project:

1. Go to your LinkedIn profile and select **Add profile section** > **Projects**
2. Title: "Enterprise Administration Across Seven Domains — Mastering GitHub Specialization"
3. Description: Summarize the project deliverables and key skills demonstrated
4. Link: Include the URL to your completed GitHub repository
