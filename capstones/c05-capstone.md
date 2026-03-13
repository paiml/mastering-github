# Capstone: Evaluating and Integrating AI Models

## Project Overview

A product team is building an AI-powered customer support assistant and needs to select the right model from GitHub Models, manage API rate limits and token budgets for production scale, and build an HTTP API that serves model responses. Evaluate candidate models in the GitHub Models playground, implement a rate-limit-aware integration, and deploy a working API endpoint that demonstrates the full model-to-production pipeline.

## Deliverables

### 1. Evaluate and Select a Model from GitHub Models

Navigate the GitHub Models marketplace and filter models by task type, parameter count, and license. Use the playground to test at least three candidate models with the same prompt — compare response quality, latency, and token usage. Apply responsible AI evaluation criteria including content filtering, bias detection, and safety guardrails. Produce a one-page model comparison matrix documenting which model best fits the customer support use case and why, with specific playground results as evidence.

### 2. Implement Rate Limit Management and Scaling Strategy

Create a personal access token with scoped permissions for GitHub Models API access. Document the free tier rate limits (requests per minute, tokens per day) and design a token budget that keeps the application within limits during normal operation. Implement retry logic with exponential backoff that handles 429 responses gracefully. Produce a scaling plan that explains how to move from free tier to paid tier — including cost projections for 1,000, 10,000, and 100,000 daily requests.

### 3. Build and Test an HTTP API Integration

Set up a development environment in Codespaces with the required SDK dependencies. Build an HTTP API endpoint that accepts a user query, sends it to the selected GitHub model, and returns the response. Implement input validation and error handling for malformed requests, API failures, and rate limit exhaustion. Write tests that verify the API handles both successful responses and failure scenarios, and document the testing strategy for validating AI model output quality.

## Evaluation Criteria

### Distinction

- Produces a model comparison matrix with quantified playground results across three models, applies responsible AI criteria to the selection, and justifies the final choice with specific performance and safety evidence
- Implements rate limit handling with exponential backoff, documents free tier boundaries with token budget calculations, and produces a scaling plan with concrete cost projections across three usage tiers
- Builds a working HTTP API with input validation, structured error handling for rate limits and API failures, and a test suite that covers both success and failure paths with a documented testing strategy for AI output quality

### Proficient

- Compares models in the playground and selects one with a stated rationale, but does not quantify the comparison or apply responsible AI evaluation criteria systematically
- Creates an API token and documents rate limits, but does not implement retry logic or produce a scaling cost projection
- Builds an API endpoint that returns model responses, but lacks structured error handling or tests for failure scenarios

### Developing

- Explores the GitHub Models marketplace but does not conduct a systematic comparison or document the selection rationale
- Creates an API token without documenting scope, rate limits, or scaling considerations
- Attempts an API integration but the endpoint does not handle errors or validate input
