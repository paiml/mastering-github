# Capstone: From Zero to Pull Request

## Project Overview

Build a collaborative open-source documentation site from scratch. Starting with an empty GitHub account, create a repository, establish a branching workflow, and simulate a three-person team collaboration using issues, pull requests, and a fork-based contribution model. The project produces a GitHub Pages site with at least four merged pull requests and a fully triaged issue board.

## Deliverables

### 1. Create a Repository with Professional Configuration

Initialize a public repository with a README that describes the project, a `.gitignore` tailored to the chosen static site generator (Jekyll, Hugo, or plain HTML), and an appropriate open-source license. The initial commit history should contain at least three atomic commits — one for each file — rather than a single bulk commit. Enable GitHub Pages from the `main` branch.

### 2. Implement a Branch-PR-Merge Workflow with Code Review

Create four feature branches, each adding a distinct page or section to the site. Each branch must result in a pull request with a descriptive title, body referencing the related issue number, and at least one review comment (self-review is acceptable for solo learners). Merge two PRs using merge commits and two using squash merges, then explain in the README which strategy suits which scenario.

### 3. Design a Project Board with Issues and Milestones

Create at least six issues organized across two milestones — "v1.0 Launch" and "v1.1 Improvements." Apply at least three custom labels (e.g., `content`, `bug`, `enhancement`) and assign issues to the project board with columns for To Do, In Progress, and Done. Fork the repository from a second GitHub account (or have a peer fork it), submit a pull request from the fork, and merge it into the upstream repository.

## Evaluation Criteria

### Distinction

- Commit messages follow a consistent convention (e.g., conventional commits) and each commit represents a single logical change
- README explains the trade-offs between merge commit, squash, and rebase strategies with concrete examples from the project's own PR history
- The fork-based contribution includes a merge conflict that was resolved correctly, with the resolution documented in the PR conversation

### Proficient

- Repository contains README, `.gitignore`, and license with GitHub Pages deployed and accessible
- All four pull requests are merged with descriptive bodies referencing issue numbers
- Project board reflects accurate issue state with labels and milestone assignment

### Developing

- Repository exists but `.gitignore` or license is missing or generic
- Pull requests are merged without descriptions or issue references
- Issues exist but lack labels, milestones, or project board organization
