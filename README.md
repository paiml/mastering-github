# Mastering GitHub

<p align="center">
  <img src="assets/hero.svg" alt="Mastering GitHub: 9-Course Specialization" width="100%"/>
</p>

**From First Commit to Production Applications** — a 9-course Coursera specialization
that takes you from zero GitHub experience through AI-assisted development to
building production applications with GitHub Copilot and AI agents.

## Courses

| # | Course | Focus | Capstone | Labs |
|---|--------|-------|----------|------|
| 1 | **From Zero to Pull Request** | Git workflow, branches, PRs, issues, forks, AI agents | [Capstone](capstones/c01-capstone.md) | — |
| 2 | **Security, Identity, and Access** | 2FA, SSH keys, repository visibility, org policies | [Capstone](capstones/c02-capstone.md) | — |
| 3 | **Codespaces, Actions, and Ecosystem Tools** | Cloud IDEs, GPU instances, CI/CD, Copilot | [Capstone](capstones/c03-capstone.md) | — |
| 4 | **Enterprise Administration Across Seven Domains** | Org management, RBAC, compliance, audit logs | [Capstone](capstones/c04-capstone.md) | — |
| 5 | **Evaluating and Integrating AI Models** | GitHub Models, API tokens, model comparison | [Capstone](capstones/c05-capstone.md) | — |
| 6 | **Advanced Prompt Engineering for Code** | Multi-file context, slash commands, Copilot Chat | [Capstone](capstones/c06-capstone.md) | [Labs](https://github.com/paiml/advanced-prompting-with-github-copilot) |
| 7 | **AI-Augmented Testing and Refactoring** | Test generation, code review, refactoring patterns | [Capstone](capstones/c07-capstone.md) | [Labs](https://github.com/paiml/ghcp-for-systems-level-development) |
| 8 | **Governing AI-Generated Code** | Security audit, license compliance, responsible AI | [Capstone](capstones/c08-capstone.md) | [Labs](https://github.com/paiml/responsible-ai-dev) |
| 9 | **Production Application Capstone** | End-to-end project integrating all specialization skills | [Capstone](capstones/c09-capstone.md) | [Labs](https://github.com/paiml/GitHub-Copilot-Mastery-Capstone) |

## Repositories

All course code and labs live in public GitHub repositories under the [paiml](https://github.com/paiml) organization.

| Repository | Courses | Description |
|-----------|---------|-------------|
| [mastering-github](https://github.com/paiml/mastering-github) | 1–5 | Main specialization repo — capstone projects, course structure |
| [advanced-prompting-with-github-copilot](https://github.com/paiml/advanced-prompting-with-github-copilot) | 6 | Labs for multi-turn prompting, context scaffolding, conversational AI |
| [ghcp-for-systems-level-development](https://github.com/paiml/ghcp-for-systems-level-development) | 7 | Labs for AI-assisted TDD, large-scale refactoring, infrastructure as code |
| [responsible-ai-dev](https://github.com/paiml/responsible-ai-dev) | 8 | Labs for validating AI-generated code, custom instructions, model selection |
| [GitHub-Copilot-Mastery-Capstone](https://github.com/paiml/GitHub-Copilot-Mastery-Capstone) | 9 | Capstone project — full-stack production application with Copilot |
| [ruchy-docker](https://github.com/paiml/ruchy-docker) | 9 | Reference project — Docker benchmarking (used in capstone) |
| [ruchy-lambda](https://github.com/paiml/ruchy-lambda) | 9 | Reference project — AWS Lambda performance (used in capstone) |

## Capstone Projects

<p align="center">
  <img src="capstones/banner.svg" alt="Capstone Projects" width="100%"/>
</p>

Each course includes a hands-on capstone project that integrates all modules into a realistic scenario. Completed capstones can be shared on LinkedIn as portfolio projects. See the [capstones/](capstones/) directory.

## Installation

```bash
git clone https://github.com/paiml/mastering-github.git
cd mastering-github
make check
```

## Usage

```bash
make help          # Show available commands
make lint          # Lint markdown files
make test          # Validate course structure (9 courses, capstone sections)
make check         # Run lint + test
```

## Structure

Each course is ~60 minutes of 3–5 minute videos organized as:

**Course → Module → Lesson (3–5 videos) → Key Terms + Reflection**

Every module ends with a **Critical Thinking Assessment** (quiz + role-play practice assignment).

## Instructors

- **Liam Parker** — Educator · Developer tools, cloud platforms, AI-assisted development
- **Noah Gift** — Founder, Pragmatic AI Labs · Duke University
- **Alfredo Deza** — Author and content creator · Python, Rust, DevOps, ML

## License

Course content copyright Pragmatic AI Labs. Code examples are MIT licensed.
