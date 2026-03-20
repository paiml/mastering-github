# Capstone: Governing AI-Generated Code

## Project Overview

A healthcare startup is adopting GitHub Copilot for its development team but faces strict regulatory requirements — all AI-generated code must be validated for security vulnerabilities, logical correctness, and compliance with internal coding standards before merging. Design and implement a governance framework that combines automated validation, security auditing, custom Copilot configurations, and informed LLM selection to ensure AI-generated code meets production quality standards.

## Deliverables

### 1. Build a Security Audit Workflow for AI-Generated Code

Generate code with GitHub Copilot for a data processing module that handles sensitive patient records. Apply systematic verification techniques — static analysis, manual review, and runtime testing — to identify security vulnerabilities, logical flaws, and hallucinated APIs in the generated output. Use OWASP patterns to check for injection vulnerabilities, broken access control, and data exposure risks. Document each finding with the detection method, severity, and remediation applied. Produce a security audit report that traces every AI-generated function from initial output through verification to approved version.

### 2. Configure Custom Copilot Instructions and Team Standards

Create a copilot-instructions.md file that enforces the startup's coding standards — input validation on all public functions, structured error handling patterns, no hardcoded credentials, and mandatory type annotations. Test the custom configuration by generating code with and without the instructions file active, documenting how the output quality changes. Create additional custom rules for domain-specific requirements (e.g., HIPAA-relevant logging constraints, data anonymization patterns). Demonstrate that Copilot's suggestions change measurably when custom instructions are applied.

### 3. Evaluate LLMs and Recommend a Model Strategy

Compare at least three language models available through GitHub Copilot on the same set of coding tasks — measure code correctness, security posture, adherence to custom instructions, and response latency. Use code generation benchmarks to quantify performance differences. Produce a cost-benefit analysis that recommends which model to use for different task types (routine implementation, security-sensitive code, complex algorithms). Document the trade-offs between model capability, cost, and speed, and propose a model selection policy for the development team.

## Evaluation Criteria

### Distinction

- Produces a comprehensive security audit with OWASP-pattern detection, hallucinated API identification, and a traceable remediation chain from initial AI output to approved code, with severity-based prioritization
- Demonstrates measurable improvement in AI output quality with copilot-instructions.md active versus inactive, including domain-specific rules for regulatory compliance, with before/after code samples as evidence
- Compares three models with quantified benchmarks across correctness, security, cost, and latency dimensions, producing a task-specific model selection policy with justified recommendations

### Proficient

- Identifies security vulnerabilities and logical flaws in AI-generated code using static analysis and manual review, but does not systematically apply OWASP patterns or trace the full remediation chain
- Creates copilot-instructions.md with coding standards and demonstrates Copilot behavior changes, but does not create domain-specific rules or quantify the improvement
- Compares models on code generation tasks and recommends one, but does not quantify the comparison across multiple dimensions or produce a task-specific selection policy

### Developing

- Reviews AI-generated code and identifies some issues but without a systematic audit methodology or documentation of findings
- Creates a copilot-instructions.md file but does not test its effect on Copilot output or document the configuration strategy
- References different LLMs but does not conduct a structured comparison or justify the selection

## Share Your Work

Add this capstone to your LinkedIn profile as a portfolio project:

1. Go to your LinkedIn profile and select **Add profile section** > **Projects**
2. Title: "Governing AI-Generated Code — Mastering GitHub Specialization"
3. Description: Summarize the project deliverables and key skills demonstrated
4. Link: Include the URL to your completed GitHub repository
