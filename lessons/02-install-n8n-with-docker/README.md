# Lesson 2 · Install n8n with Docker

▶ [Watch this lesson](https://youtu.be/nRxDPfsSjk0?t=185) (starts at 3:05)

## Goal

Lesson two. Install n8n with Docker.

## In this lesson

```bash
docker --version
docker compose version
curl -fsSL https://get.n8n.io | sh
cd n8n && ls -a
docker compose ps --format "table {{.Service}}\t{{.Status}}"
```

Then open http://localhost:5678 and set up the owner account (it stays on your machine). Everyday commands: `docker compose -f ./n8n/compose.yml down` (stop), `... up -d` (start), `curl -fsSL https://get.n8n.io | sh -s -- --upgrade` (upgrade). Careful: `down -v` deletes all your n8n data.

## Recap

So: one command with Docker installs n8n. It runs on localhost, port fifty six seventy eight. And the owner account stays on your machine. Time for the first workflow.
