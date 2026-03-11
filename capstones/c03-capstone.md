# Capstone: Codespaces, Actions, and Ecosystem Tools

## Project Overview

A machine learning team needs a reproducible development environment that provisions GPU-capable Codespaces for model fine-tuning, automates CI/CD with GitHub Actions, and integrates Copilot for code assistance. Build the complete developer platform for a sample repository — from dev container configuration through automated testing to a working Actions pipeline.

## Deliverables

### 1. Build a Dev Container with Codespaces Configuration

Create a repository with a `.devcontainer/devcontainer.json` that specifies a GPU-enabled machine type, installs Python and ML dependencies (PyTorch or Hugging Face Transformers), and applies dotfiles for shell customization. Launch the Codespace and verify that the GPU is accessible and the development environment matches the configuration. Document the machine type selection, idle timeout, and retention settings appropriate for controlling cloud compute costs.

### 2. Implement a GitHub Actions CI/CD Pipeline

Create a `.github/workflows/ci.yml` that triggers on push and pull request events. The workflow should install dependencies, run a linter, execute a test suite, and produce a build artifact. Add a second workflow or job that runs only on the main branch to simulate a deployment step. Use repository secrets for any credentials and demonstrate caching of dependencies to reduce build time.

### 3. Integrate Copilot and Demonstrate AI-Assisted Development

Use GitHub Copilot Chat to generate a Python function (e.g., a data preprocessing utility or model inference wrapper) and document the prompt used and the output received. Use Copilot CLI to construct a Git command or shell one-liner from a natural language description. Compare the Chat and CLI interaction models — describe when each is more effective and what context each requires to produce accurate suggestions.

## Evaluation Criteria

### Distinction

- Dev container configuration specifies GPU machine type, pins dependency versions, configures dotfiles, and documents cost-control settings (idle timeout, billing limits) with rationale for each choice
- Actions pipeline uses matrix builds or multi-job workflows, caches dependencies, stores artifacts, uses repository secrets securely, and demonstrates conditional deployment logic on the main branch
- Copilot comparison goes beyond surface-level description to evaluate accuracy, context window limitations, and the tradeoff between Chat (multi-turn, workspace-aware) and CLI (single-shot, terminal-scoped) for different development tasks

### Proficient

- Creates a working Codespace with a dev container that installs the correct dependencies and launches successfully, but does not address GPU configuration or cost controls
- Actions workflow triggers correctly, runs tests, and passes on push, but uses a single job without caching, artifacts, or conditional deployment
- Uses Copilot to generate code and documents the prompt, but does not compare Chat and CLI or evaluate the quality of the generated output

### Developing

- Attempts a dev container configuration but the Codespace fails to build or is missing key dependencies
- Creates a workflow file that does not trigger correctly or fails on execution without diagnosis
- Mentions Copilot features without demonstrating actual usage or documenting prompts and outputs
