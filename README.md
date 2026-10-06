# ThePoet

**Multi-agent AI orchestration experiment for coordinating specialized agents around business and technical workflows.**

TypeScript-based prototype exploring task routing, agent specialization, shared context, structured outputs, and multi-provider LLM integration.

> **Status honesty:** Experimental / portfolio project. Previous production-scale, latency, and concurrency claims are not used here. Source code is the authority for implementation status.

## Problem

Complex work often needs multiple specialized perspectives (technical, operational, legal, product). Orchestrating several LLM-backed agents with clear routing, shared context, and failure isolation is harder than a single chat completion — and easy to over-claim.

## Solution

ThePoet explores:

- Specialized agent roles
- Task routing into workflows
- Context / memory sharing concepts
- Structured outputs
- Multi-provider LLM abstraction (OpenAI, Anthropic, Ollama concepts)
- CLI and API entry points

A stronger, accurate description: *a multi-agent orchestration prototype exploring task routing, specialized agents, shared context, and model-provider abstraction.*

## Architecture

```
User / CLI / API
       │
   Task Router
       │
  Agent Workflow
       │
Specialized Agents
       │
 LLM Provider(s)
       │
 Context / Memory
```

Documented role ideas have included executive/functional agents (e.g. technical, operations, compliance). Treat roles as design, not proof of production autonomy.

## Features

- Agent specialization and task routing concepts
- Multi-agent workflow design
- LLM provider integration patterns
- Context / memory concepts (Redis / PostgreSQL referenced)
- CLI and REST-oriented interfaces
- Structured output handling

## Tech stack

| Area | Technology |
|------|------------|
| Language | TypeScript |
| Runtime | Node.js |
| Models | OpenAI, Anthropic, Ollama (as referenced) |
| Data concepts | Redis, PostgreSQL |
| Interfaces | REST API, CLI; Telegram / GitHub integration concepts |

## Repository structure

Inspect the repository tree for agents, router, providers, and API/CLI entrypoints. Prefer code over this summary when details differ.

## Installation

```bash
git clone https://github.com/lukewealth/ThePoet.git
cd ThePoet
npm install   # or the package manager indicated by lockfiles
cp .env.example .env   # if present
```

## Environment variables

Typical needs (confirm against `.env.example` if present):

- LLM provider API keys
- Optional Redis / PostgreSQL connection strings
- Any integration tokens (GitHub, Telegram, etc.)

Never commit real secrets.

## Usage

Use the project’s documented scripts for CLI or API. Prefer non-production keys and explicit tool permissions when experimenting with agents that call external systems.

## Testing

Check the repo for test suites. If minimal, verification is primarily manual and type-level until tests are expanded.

## Deployment

Not presented as a production SaaS. Suitable for local demos and architecture discussion.

## Security

- Secrets via environment only
- Isolate provider failures; avoid cascading agent errors
- Constrain tool permissions and outbound actions
- Consider prompt-injection and untrusted content in agent inputs

## Limitations

- Prototype / experimental scope
- No verified production SLAs, token capacity claims, or business-scale metrics in this README
- Memory and integration depth must be verified in code
- Not a compliance-certified system

## Current status

**Experimental / portfolio project.**  
Useful interview discussion areas: task routing, agent state, context sharing, failure isolation, retries/idempotency, evaluation, and secret/tool permission design.

## Roadmap

- Stronger evaluation harness for agent behaviour
- Clearer implemented-vs-design documentation
- Hardened tool allow-lists and audit logging
- Automated tests for router and agent contracts

## Keywords

`ai` `artificial-intelligence` `agentic-ai` `ai-agents` `llm` `typescript` `nodejs` `backend` `api` `automation` `software-architecture` `multi-agent` `orchestration`

## License

See repository license file if present; otherwise all rights reserved by the author.
