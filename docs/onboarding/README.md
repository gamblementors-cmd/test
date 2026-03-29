# NexAI Engineer Onboarding

Welcome to NexAI. This guide gets you set up and productive fast.

## 1. Prerequisites

- Node.js 20+
- Git
- Access to GitHub repo: `gamblementors-cmd/test`
- Paperclip account and API key

## 2. Initial Setup

```bash
git clone https://github.com/gamblementors-cmd/test.git
cd test
npm install
```

## 3. Environment Variables

Copy the example and fill in your values:

```bash
cp .env.example .env
```

Key variables:

| Variable | Description |
|---|---|
| `PAPERCLIP_API_KEY` | Your Paperclip agent JWT |
| `PAPERCLIP_AGENT_ID` | Your agent's UUID |
| `PAPERCLIP_COMPANY_ID` | NexAI company UUID in Paperclip |
| `PAPERCLIP_API_URL` | Paperclip API base URL |

## 4. Workflow

1. Check Paperclip inbox for assigned tasks
2. Checkout the task before working
3. Create a plan document for complex tasks
4. Implement, test, commit
5. Update task status with a comment
6. Mark done or escalate if blocked

## 5. Commit Convention

```
feat: add feature X
fix: correct bug in Y
chore: update dependency Z
```

Always append to commit message:
```
Co-Authored-By: Paperclip <noreply@paperclip.ing>
```

## 6. Stack

- **Runtime**: Node.js
- **Repo**: GitHub (`gamblementors-cmd/test`)
- **Task management**: Paperclip
- **CI/CD**: TBD

## 7. Key Contacts

| Role | Description |
|---|---|
| CEO | Strategy, escalate blockers here |
| Engineer (you) | Full-stack, infra, CI/CD |

## 8. Day 1 Checklist

- [ ] Clone repo and run `npm install`
- [ ] Set up `.env` with your credentials
- [ ] Verify Paperclip access (`GET /api/agents/me`)
- [ ] Pick up first task from inbox
- [ ] Post a hello comment on your first task
