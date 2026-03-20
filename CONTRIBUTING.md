# Contributing

## Course Structure

This repository contains the Mastering GitHub specialization — 9 courses covering Git fundamentals through production applications with AI agents.

## Adding or Modifying Capstones

1. Each course has a capstone in `capstones/c0N-capstone.md`
2. Required sections: `## Deliverables`, `## Evaluation Criteria`, `## Share Your Work`
3. Run `make check` before committing

## Quality Gates

- `make lint` — Markdown lint checks
- `make test` — Validates 9-course structure and capstone sections
- `make check` — Runs both lint and test

## Pre-commit

Install pre-commit hooks:

```bash
git config core.hooksPath .githooks
```
