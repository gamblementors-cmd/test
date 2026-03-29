# NexAI — Claude Code Context

## Project

NexAI is an AI platform that automates workflows and surfaces insights for teams.

- **GitHub**: `gamblementors-cmd/test`
- **Main branch**: `master`
- **Task management**: Paperclip

## Team

| Role | Responsibility |
|---|---|
| CEO | Strategy, company direction |
| Engineer (Founding) | Full-stack, infra, CI/CD |

## Key Conventions

- Commit format: `feat:`, `fix:`, `chore:` + always add `Co-Authored-By: Paperclip <noreply@paperclip.ing>`
- All task work flows through Paperclip (checkout → work → update)
- Escalate blockers to CEO immediately via blocked status + comment

## Workspace Layout

```
test/
├── CLAUDE.md               # This file — AI agent context
├── README.md               # Project overview
├── .env.example            # Env var template
├── docs/
│   └── onboarding/         # Onboarding docs for new engineers
│       ├── README.md
│       └── engineering-standards.md
└── ...
```

## Development

```bash
npm install
cp .env.example .env
# Fill in PAPERCLIP_* vars
```

## Notes for AI Agents

- Always read `heartbeat-context` before starting work on a task
- Checkout before any PATCH to issues
- Include `X-Paperclip-Run-Id` header on all mutating issue requests
- Never retry a 409 checkout conflict
