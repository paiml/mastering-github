# Capstone: Codespaces, Actions, and Ecosystem Tools

## Project Overview

A machine learning team needs a reproducible development environment that provisions GPU-capable Codespaces for model fine-tuning, automates CI/CD with GitHub Actions, and integrates Copilot for code assistance. Build the complete developer platform for a sample repository — from dev container configuration through automated testing to a working Actions pipeline.

## Deliverables

### 1. Build a Dev Container with Codespaces Configuration

Create a repository with a `.devcontainer/devcontainer.json` that specifies a GPU-enabled machine type and installs Python and ML dependencies (Hugging Face Transformers). Configure a dotfiles repository with shell aliases and link it in Codespaces account settings so customizations persist automatically across all new Codespaces. Launch the Codespace and verify that the GPU is accessible and the development environment matches the configuration.

### 2. Implement a GitHub Actions CI/CD Pipeline

Create a `.github/workflows/ci.yml` that triggers on push and pull request events. The workflow should install dependencies using `make install`, run a linter with `make lint`, and execute a test suite with `make test`. Add a deployment step using `make deploy` that runs on the main branch to simulate a production release, matching the same Makefile targets used locally in the Codespace.

### 3. Integrate Copilot and Demonstrate AI-Assisted Development

Use GitHub Copilot Chat to generate a Python function (such as a data preprocessing utility or a Click-based CLI tool) and document the prompt used and the output received. Use Copilot CLI to construct a shell command from a natural language description using the `??` syntax. Compare the Chat and CLI interaction models — describe when each is more effective and what context each requires to produce accurate suggestions. Combine the generated code with your Makefile and Actions pipeline to demonstrate an end-to-end Python DevOps workflow integrating Copilot, Actions, and Codespaces.

## Evaluation Criteria

### Distinction

- Dev container configuration specifies GPU machine type, pins dependency versions, and configures dotfiles via Codespaces account settings — with clear justification for machine type selection relative to the ML workload
- Actions pipeline uses a Makefile-linked workflow with `make install`, `make lint`, `make test`, and `make deploy` steps on `ubuntu-latest`, demonstrating that identical commands run locally in the Codespace and remotely in the CI environment
- Copilot comparison articulates specific scenarios where Chat (conversational, editor-based, multi-turn) and CLI (`??` syntax, terminal-scoped, single-shot) each excel, with concrete examples from the development workflow

### Proficient

- Creates a working Codespace with a dev container that installs the correct dependencies and launches successfully on a GPU machine type, but does not configure dotfiles or justify the machine type selection
- Actions workflow triggers correctly and runs Makefile targets on push, but does not include a deployment step or demonstrate Makefile-to-Actions correspondence
- Uses Copilot to generate code and documents the prompt, but does not compare Chat and CLI interaction models

### Developing

- Attempts a dev container configuration but the Codespace fails to build or is missing key dependencies
- Creates a workflow file that does not trigger correctly or fails on execution without diagnosis
- Mentions Copilot features without demonstrating actual usage or documenting prompts and outputs
