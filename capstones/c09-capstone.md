# Capstone: Autonomous Agent Workflows

## Project Overview

A DevOps team wants to reduce manual intervention in their software delivery pipeline by deploying autonomous GitHub Copilot agents that handle multi-step tasks — from issue triage through code generation to pull request review. Design and implement an agent-powered workflow that uses Copilot agents, Model Context Protocol (MCP) servers, and multi-step automation to autonomously process development tasks with human oversight at critical checkpoints.

## Deliverables

### 1. Configure Copilot Agent Mode for Multi-Step Automation

Set up GitHub Copilot in Agent mode and configure it to execute multi-step development tasks autonomously — reading issue descriptions, navigating the codebase, generating implementation code, writing tests, and creating pull requests. Define the agent's tool access permissions and document which operations require human approval versus autonomous execution. Demonstrate the agent completing an end-to-end task: from a GitHub issue describing a bug fix through code change, test generation, and PR creation. Document the agent's decision-making at each step and where it required course correction.

### 2. Integrate MCP Servers for External Tool Access

Configure a Model Context Protocol server that gives the Copilot agent access to external tools — a project management system for reading task context, a documentation server for referencing API specifications, and a testing harness for validating generated code. Document the MCP server configuration including tool definitions, authentication, and permission boundaries. Demonstrate the agent using MCP tools to gather context before generating code and to validate its output after generation. Explain how MCP extends the agent's capabilities beyond the repository and what security boundaries must be maintained.

### 3. Design a Human-in-the-Loop Agent Workflow

Create a complete agent workflow definition that processes incoming GitHub issues through classification, implementation planning, code generation, testing, and review — with human approval gates at specified checkpoints. Define escalation criteria for when the agent should stop and request human intervention (ambiguous requirements, security-sensitive changes, breaking API modifications). Implement the workflow for a sample repository and process at least three issues of varying complexity. Produce a workflow diagram and a post-mortem analysis that evaluates agent accuracy, time saved versus manual development, and recommendations for expanding autonomous scope.

## Evaluation Criteria

### Distinction

- Demonstrates Agent mode completing an end-to-end issue-to-PR workflow with documented decision points, tool permission boundaries, and specific examples of autonomous versus human-approved operations
- Configures MCP servers with external tool integrations, demonstrates context gathering and output validation through MCP tools, and documents security boundaries with justified permission scoping
- Produces a workflow with defined escalation criteria, processes three issues of varying complexity, and includes a post-mortem with quantified time savings and accuracy metrics

### Proficient

- Configures Agent mode and demonstrates multi-step task completion, but does not document decision-making at each step or define clear permission boundaries
- Sets up an MCP server with basic tool access, but does not demonstrate the agent using external tools for context gathering or output validation
- Creates a workflow with human checkpoints, but does not define escalation criteria or analyze agent performance across multiple issues

### Developing

- References Copilot Agent mode and MCP without demonstrating a working multi-step automation
- Describes MCP server concepts but does not implement or configure tool integrations
- Outlines a workflow without processing actual issues or evaluating agent performance
