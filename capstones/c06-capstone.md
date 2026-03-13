# Capstone: Advanced Prompt Engineering for Code

## Project Overview

A development team is onboarding to a legacy Python codebase with no documentation, inconsistent patterns, and no test coverage. Using GitHub Copilot's conversational prompting, iterative refinement, and multi-file context techniques, reverse-engineer the codebase, generate API documentation, and refactor a key module — demonstrating the full advanced prompting workflow from exploration through production-quality output.

## Deliverables

### 1. Explore an Unknown Codebase Using Conversational Prompting

Use GitHub Copilot Chat to navigate the codebase — start with @workspace queries to understand the project structure, then use #file references to examine specific modules. Conduct a multi-turn conversation that progressively narrows from architecture overview to function-level understanding. Compare Ask, Edit, and Agent modes for codebase exploration and document which mode is most effective at each level of detail. Produce a codebase map that describes the module hierarchy, key dependencies, and data flow — generated entirely through Copilot interactions.

### 2. Generate API Documentation and Code from Specifications

Select a module with undocumented public functions and use Copilot Chat to generate API documentation from the existing code. Then reverse the workflow — write an API specification for a new endpoint and use Copilot to generate the implementation code from that specification. Leverage open editor tabs as context to ensure generated code matches existing patterns and import conventions. Document the iterative refinement steps taken to improve both the documentation and the generated code from first draft to final version.

### 3. Refactor a Module Using Multi-File Context and Iterative Refinement

Identify a module with code quality issues (e.g., duplicated logic, inconsistent naming, missing error handling). Provide context from multiple files using #file markers and @workspace references so Copilot understands cross-file dependencies. Execute the refactoring in a multi-turn conversation — start with a broad plan, then iteratively refine each change. Demonstrate at least three refinement cycles where Copilot output is improved through follow-up prompts. Document the prompt strategy and explain why each refinement was necessary.

## Evaluation Criteria

### Distinction

- Multi-turn exploration produces a comprehensive codebase map with architecture, dependencies, and data flow — with documented comparison of Ask, Edit, and Agent modes showing when each excels
- Demonstrates both code-to-documentation and specification-to-code workflows with iterative refinement from first draft to final version, leveraging open tabs for pattern-consistent output
- Executes a multi-file refactoring with three or more documented refinement cycles, using #file and @workspace context to maintain cross-file consistency, with clear justification for each prompt iteration

### Proficient

- Uses Copilot Chat to explore the codebase and produces a structural overview, but does not compare interaction modes or document the progressive narrowing strategy
- Generates API documentation or implementation code but does not demonstrate both directions of the workflow or document iterative refinement steps
- Refactors a module with Copilot assistance but does not use multi-file context or demonstrate multiple refinement cycles

### Developing

- Asks Copilot about the codebase but does not structure the exploration or produce a coherent codebase map
- Generates documentation or code without iterative refinement or cross-file context awareness
- Attempts refactoring without leveraging workspace context or documenting the prompt strategy
