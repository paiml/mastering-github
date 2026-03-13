# Capstone: Production Application Capstone

## Project Overview

Build a complete production-quality web application from scratch using GitHub Copilot across every phase of development — project planning, API implementation, business logic, data persistence with an ORM, comprehensive testing, and code review. This capstone integrates all skills from the specialization: Git workflow, security practices, CI/CD with Actions, AI-assisted development, and code governance into a single end-to-end project.

## Deliverables

### 1. Plan the Application and Establish Project Infrastructure

Use GitHub Copilot to scope the project — define the domain model, API endpoints, and data layer architecture through conversational prompting. Query internal knowledge bases and documentation to inform design decisions. Create the repository with professional configuration: README, .gitignore, license, branch protection rules, and a GitHub Actions CI pipeline that runs linting and tests on every pull request. Produce an architecture document generated through Copilot Chat that maps the API layer, business logic layer, and data persistence layer with their dependencies.

### 2. Implement the Full Application Stack with AI Assistance

Build the API layer with endpoints for CRUD operations, implementing input validation and structured error handling. Code the business logic layer with complex rules (e.g., authorization checks, data transformation, workflow state transitions) using Copilot's multi-file context to maintain consistency across modules. Implement the data persistence layer using an ORM with migrations, relationships, and query optimization. Use iterative refinement — generate initial implementations with Copilot, review for quality, and refine through multi-turn conversations until the code meets production standards.

### 3. Test, Review, and Deliver a Production-Ready Application

Build a comprehensive test suite spanning unit tests (isolated business logic), integration tests (API endpoints with database), and end-to-end tests (full request lifecycle). Use Copilot to generate test cases including edge cases and boundary conditions, then evaluate coverage and fill gaps. Conduct a code review of the AI-generated implementation — identify any security vulnerabilities, hallucinated APIs, or logical flaws using the governance techniques from Course 8. Produce a final pull request with a detailed description that documents the development process, Copilot's contribution at each phase, and lessons learned about AI-assisted production development.

## Evaluation Criteria

### Distinction

- Architecture document traces design decisions through Copilot conversations, CI pipeline enforces quality gates on every PR, and repository configuration reflects security best practices from across the specialization
- Implements all three layers with cross-module consistency maintained through multi-file context, iterative refinement documented across multiple cycles, and business logic handling complex rules correctly
- Test suite achieves 80%+ coverage spanning unit, integration, and end-to-end tests, code review identifies and remediates AI-generated defects, and the final PR documents the complete AI-assisted development workflow

### Proficient

- Creates a repository with CI pipeline and produces an architecture plan with Copilot, but does not document the conversational planning process or configure branch protection
- Implements API, business logic, and data layers that function correctly, but does not demonstrate iterative refinement or cross-module consistency through multi-file context
- Writes tests that cover the main functionality and submits a PR, but does not conduct a governance-informed code review or document Copilot's role in the development process

### Developing

- Creates a repository without CI configuration or architecture planning, jumping directly to implementation
- Implements partial functionality without structured layering or AI-assisted refinement
- Minimal or no test coverage, with the PR lacking description or review of AI-generated code quality
