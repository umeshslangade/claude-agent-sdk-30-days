# Day 01: Why I'm building AI agents in public

**Goal:** set up the toolchain so Day 3's first agent runs in one command.

## Run it (environment check)

```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env                                  # then add your ANTHROPIC_API_KEY
python -c "import claude_agent_sdk; print('claude-agent-sdk ready')"
```

## Why I'm doing this

- I design Azure solutions for a living. Agents are becoming a workload I need to architect, secure and run.
- Learning in public forces me to understand each concept well enough to explain it.
- Every day gets runnable code plus an **Azure angle**: identity, secrets, networking and cost.

## What's coming

Week 1 covers the agent loop, a first agent, least privilege, permission modes and reading the message stream. See the [daily index](../README.md#daily-index).

## Common mistake

Committing `.env`. It's in `.gitignore` already, and push protection is on for this account, but check `git status` before every commit.
