# Lesson 7 · Turn your agent into an API

▶ [Watch this lesson](https://youtu.be/nRxDPfsSjk0?t=1033) (starts at 17:13)

## Goal

Lesson seven. Turn your agent into an API.

## In this lesson

Import [`app/workflows/04-support-triage.json`](../../app/workflows/04-support-triage.json): Webhook (POST `/triage`, respond using Respond to Webhook) → AI Agent with a Structured Output Parser → Respond to Webhook. **Publish** it and call it:

```bash
curl -s -X POST http://localhost:5678/webhook/triage -H "Content-Type: application/json" -d '{"message": "Hi, I was charged twice for my order #1042. Can you refund one of the payments?"}' | jq
```

## Recap

So: a webhook turns a workflow into an API endpoint. The output parser gives you clean JSON. And the executions tab logs every call.
