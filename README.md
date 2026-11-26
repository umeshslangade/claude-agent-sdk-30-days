# 🤖 Claude Agent SDK: 30 Days of Practical AI Agents

> One small, runnable agent per day. Each folder matches a LinkedIn post.

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?logo=python&logoColor=white)
![Claude Agent SDK](https://img.shields.io/badge/Claude%20Agent%20SDK-D97757?logo=anthropic&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Last commit](https://img.shields.io/github/last-commit/umeshslangade/claude-agent-sdk-30-days)

## Why this repo

Most agent tutorials stop at "hello world". This repo goes from a first agent to tools, MCP servers, memory, sub-agents, evals and deployment on Azure, one day at a time, with the trade-offs written down.

## Daily index

| Day | Date | Topic | Folder | Post |
|---|---|---|---|---|
| 01 | 30 Nov | Why I'm building AI agents in public | `day-01-why-i-m-building-ai` | ⏳ |
| 02 | 01 Dec | The agent loop | `day-02-the-agent-loop` | ⏳ |
| 03 | 02 Dec | My first agent in ~20 lines | `day-03-my-first-agent-in-20` | ⏳ |
| 04 | 03 Dec | Least privilege: a read-only reviewer agent | `day-04-least-privilege-a-read-only` | ⏳ |
| 05 | 04 Dec | Permission modes | `day-05-permission-modes` | ⏳ |
| 06 | 05 Dec | Reading the message stream (and the cost) | `day-06-reading-the-message-stream` | ⏳ |
| 07 | 06 Dec | Week 1 recap | `day-07-week-1-recap` | ⏳ |
| 08 | 07 Dec | System prompts and CLAUDE.md | `day-08-system-prompts-and-claude-md` | ⏳ |
| 09 | 08 Dec | My first custom tool | `day-09-my-first-custom-tool` | ⏳ |
| 10 | 09 Dec | Designing tools the agent uses well | `day-10-designing-tools-the-agent-uses` | ⏳ |
| 11 | 10 Dec | Plugging into external MCP servers | `day-11-plugging-into-external-mcp-servers` | ⏳ |
| 12 | 11 Dec | Hooks: blocking destructive commands | `day-12-hooks-blocking-destructive-commands` | ⏳ |
| 13 | 12 Dec | Audit logging with PostToolUse | `day-13-audit-logging-with-posttooluse` | ⏳ |
| 14 | 13 Dec | Week 2 recap | `day-14-week-2-recap` | ⏳ |
| 15 | 14 Dec | Multi-turn conversations with ClaudeSDKClient | `day-15-multi-turn-conversations-with-claudesdkclient` | ⏳ |
| 16 | 15 Dec | Resume and fork sessions | `day-16-resume-and-fork-sessions` | ⏳ |
| 17 | 16 Dec | Structured output (JSON every time) | `day-17-structured-output` | ⏳ |
| 18 | 17 Dec | Subagents: splitting the work | `day-18-subagents-splitting-the-work` | ⏳ |
| 19 | 18 Dec | When NOT to use subagents | `day-19-when-not-to-use-subagents` | ⏳ |
| 20 | 19 Dec | Skills: reusable know-how for agents | `day-20-skills-reusable-know-how-for` | ⏳ |
| 21 | 20 Dec | Week 3 recap | `day-21-week-3-recap` | ⏳ |
| 22 | 21 Dec | Human-in-the-loop approvals | `day-22-human-in-the-loop-approvals` | ⏳ |
| 23 | 22 Dec | Budgets and limits | `day-23-budgets-and-limits` | ⏳ |
| 24 | 23 Dec | Evaluating agents | `day-24-evaluating-agents` | ⏳ |
| 25 | 24 Dec | Observability with OpenTelemetry | `day-25-observability-with-opentelemetry` | ⏳ |
| 26 | 25 Dec | Running Claude through Microsoft Foundry | `day-26-running-claude-through-microsoft-foundry` | ⏳ |
| 27 | 26 Dec | Deploying on Azure Container Apps Jobs | `day-27-deploying-on-azure-container-apps` | ⏳ |
| 28 | 27 Dec | Securing agents on Azure | `day-28-securing-agents-on-azure` | ⏳ |
| 29 | 28 Dec | Reference architecture for agents on Azure | `day-29-reference-architecture-for-agents-on` | ⏳ |
| 30 | 29 Dec | 30-day wrap-up | `day-30-30-day-wrap-up` | ⏳ |

> ⏳ = coming soon. Each row gets a folder and a LinkedIn link on the day it's posted.

## Quick start

```bash
git clone https://github.com/umeshslangade/claude-agent-sdk-30-days.git
cd claude-agent-sdk-30-days
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env          # add ANTHROPIC_API_KEY (never commit .env)
python day-03-my-first-agent-in-20/main.py   # first code drops on Day 3
```

## Repo layout

```
day-XX-<topic>/
├── main.py        # the runnable agent
├── README.md      # what it does, what I learned, common mistake
└── requirements.txt (if extra deps)
```

## Each day's README follows this shape

1. **Goal**: one sentence
2. **Run it**: one command
3. **How it works**: short diagram or 5 bullets
4. **Common mistake**: the thing that tripped me up
5. **Azure angle**: how this would run in production (identity, secrets, networking, cost)

## Security notes

- API keys come from environment variables or Azure Key Vault, never from code.
- Tools that touch cloud resources are read-only by default.

## Follow along

New post daily on [LinkedIn](https://www.linkedin.com/in/umesh-langade-67112380/). ⭐ the repo to keep up.

## License

MIT
