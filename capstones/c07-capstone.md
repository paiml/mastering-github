# Capstone: AI-Augmented Testing and Refactoring

## Project Overview

A platform engineering team inherits a microservice with 15% test coverage, inconsistent code style, and a manually provisioned infrastructure. Using GitHub Copilot's AI-assisted TDD, system-wide refactoring, and infrastructure-as-code generation capabilities, bring the service to production readiness — comprehensive tests, clean code, and reproducible infrastructure defined in Dockerfiles and Terraform.

## Deliverables

### 1. Build a Comprehensive Test Suite Using AI-Assisted TDD

Apply test-driven development with GitHub Copilot — write tests before implementation for a new feature in the microservice. Generate unit tests that cover edge cases, boundary conditions, and parameterized scenarios. Use Copilot to create mock objects that isolate units from external dependencies (database connections, HTTP clients). Evaluate test coverage using a coverage report, identify gaps, and generate targeted additional tests to reach at least 80% line coverage. Document the TDD workflow: which prompts produced the most effective tests and where manual intervention was required.

### 2. Execute System-Wide Refactoring with Workspace Context

Use @workspace references to analyze cross-file dependencies and identify refactoring targets across the codebase. Plan a system-wide code cleanup — rename inconsistent functions, extract duplicated logic into shared utilities, and enforce a consistent error handling pattern. Use Copilot's Edit mode with #file markers to execute changes across multiple files while maintaining consistency. Apply custom guidelines via copilot-instructions.md to enforce the team's style constraints (naming conventions, import ordering, error patterns). Verify that all existing tests still pass after refactoring.

### 3. Generate Infrastructure as Code for Production Deployment

Use GitHub Copilot to generate a multi-stage Dockerfile that builds the microservice with dependency caching, runs tests in a build stage, and produces a minimal production image. Generate a Terraform module that provisions the required cloud resources (compute instance, database, load balancer) with variables for environment-specific configuration. Document Copilot's output quality — identify where generated IaC required manual correction for security best practices (non-root user, least-privilege IAM, encrypted storage). Produce a README that explains how to build, test, and deploy the service using the generated infrastructure.

## Evaluation Criteria

### Distinction

- Demonstrates full TDD cycle with tests written before implementation, mocked dependencies, parameterized scenarios, and a documented coverage progression from 15% to 80%+ with specific prompts that produced effective tests
- Executes cross-file refactoring using @workspace and #file context with copilot-instructions.md enforcing style constraints, all existing tests passing after changes, and a documented analysis of cross-file dependencies
- Generates a multi-stage Dockerfile and Terraform module with security corrections documented, environment-specific variables, and a deployment README that covers build, test, and deploy steps

### Proficient

- Generates tests with Copilot that improve coverage and uses mocks for external dependencies, but does not follow a strict TDD workflow or document the prompt strategy
- Refactors code across files with Copilot assistance but does not use copilot-instructions.md for style enforcement or analyze cross-file dependencies before making changes
- Generates a Dockerfile and Terraform configuration that work but does not address security best practices or provide environment-specific parameterization

### Developing

- Uses Copilot to generate some tests but without a coverage-driven strategy or mocking of external dependencies
- Makes isolated code changes without analyzing cross-file impact or using workspace-level context
- Attempts IaC generation but the output requires significant manual correction to be functional
