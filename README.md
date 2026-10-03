# n8n AI Agent Tutorial: Automate Anything (Self-Hosted, Free)

Companion repository for the **Code with Antonio** video course · [Watch on YouTube](https://youtu.be/nRxDPfsSjk0).

n8n AI agent tutorial: install n8n free with Docker and build AI agents that chat, use tools, run every morning and answer like an API.

## What you'll build

Your own n8n: from zero to four real automations — a weather API call, a chat assistant with memory and tools, a daily AI-news digest that saves itself, and a support-triage API.

## Lessons

| # | Lesson | Video | Folder |
|---|---|---|---|
| 1 | What is n8n? | [0:00](https://youtu.be/nRxDPfsSjk0?t=0) | [lessons/01-what-is-n8n](lessons/01-what-is-n8n) |
| 2 | Install n8n with Docker | [3:05](https://youtu.be/nRxDPfsSjk0?t=185) | [lessons/02-install-n8n-with-docker](lessons/02-install-n8n-with-docker) |
| 3 | Your first workflow | [6:15](https://youtu.be/nRxDPfsSjk0?t=375) | [lessons/03-your-first-workflow](lessons/03-your-first-workflow) |
| 4 | Your first AI agent | [8:39](https://youtu.be/nRxDPfsSjk0?t=519) | [lessons/04-your-first-ai-agent](lessons/04-your-first-ai-agent) |
| 5 | Give your agent tools | [11:39](https://youtu.be/nRxDPfsSjk0?t=699) | [lessons/05-give-your-agent-tools](lessons/05-give-your-agent-tools) |
| 6 | An agent that works while you sleep | [14:34](https://youtu.be/nRxDPfsSjk0?t=874) | [lessons/06-an-agent-that-works-while-you-sleep](lessons/06-an-agent-that-works-while-you-sleep) |
| 7 | Turn your agent into an API | [17:13](https://youtu.be/nRxDPfsSjk0?t=1033) | [lessons/07-turn-your-agent-into-an-api](lessons/07-turn-your-agent-into-an-api) |

## Requirements

- n8n 2.41.6 (Community edition, self-hosted) · one-line setup (`get.n8n.io`, Docker 29.8 + Compose v5.5) · OpenAI gpt-6-luna · Linux

## Setup

Follow the lessons in order: each `lessons/NN-*/README.md` has the exact commands and files shown in the video.

## Run the final project

```bash
# 1. Install n8n with Docker (Docker + Docker Compose v2 required); it creates ./n8n and starts it
curl -fsSL https://get.n8n.io | sh
# 2. Open http://localhost:5678 and create your local owner account
# 3. Overview → Create credential → OpenAI (paste your OpenAI API key)
# 4. New workflow → ⋯ (More actions) → Import → app/workflows/01-weather-check.json (then 02b, 03, 04)
# 5. In each OpenAI Chat Model node, select your credential; in 03, create the data table daily_digest (day, digest)
```

## Repository structure

```
README.md          this file
lessons/           one folder per lesson: goal, timestamp, commands and files exactly as in the video
app/               the final working project
assets/            thumbnail
```

## License

MIT — use it for anything, credit appreciated.

---
Generated on 2026-10-03 from the course scripts. Code with Antonio · AI tutor.