# ThePoet

**Multi-agent AI orchestration experiment**

ThePoet explores a multi-agent architecture in TypeScript for coordinating specialized AI agents around business and technical workflows.

## What it demonstrates

- Agent specialization
- Task routing
- Context sharing
- Structured outputs
- Multi-agent workflow design
- LLM provider integration
- Redis/PostgreSQL-backed memory concepts
- GitHub integration concepts
- CLI/API interfaces

The repository documentation describes specialized roles such as CEO, CTO, CFO, CMO, legal/compliance, operations, and Web3 agents.

## Architecture

```
User / CLI / API
       |
   Task Router
       |
   Agent Workflow
       |
Specialized Agents
       |
LLM Provider(s)
       |
Context / Memory
```

## Technology referenced

- Node.js
- TypeScript
- OpenAI models
- Anthropic models
- Ollama
- Redis
- PostgreSQL
- REST API
- Telegram integration
- GitHub integration

## Important scope note

The previous README used terms such as "production-ready", specific latency numbers, concurrency figures, token capacity, and business-scale examples without providing corresponding benchmark evidence.

Those claims should not be used in a CV or interview unless reproducible measurements are added to the repository.

A stronger technical presentation is:

> "A multi-agent orchestration prototype exploring task routing, specialized agents, shared context and model-provider abstraction."

## Interview discussion areas

Be ready to explain:

- how tasks are routed
- how agent state is represented
- how context is shared
- how failures are handled
- how model/provider failures are isolated
- how retries and idempotency would work
- how agent behavior would be evaluated
- how secrets and tool permissions would be controlled

## Keywords

AI Systems Engineer, Agentic AI, Multi-Agent Systems, LLM Orchestration, TypeScript, Node.js, OpenAI, Anthropic, Ollama, Redis, PostgreSQL, Task Routing, AI Automation.

## Status

Experimental / portfolio project. Current source code is the authority for implementation status.
