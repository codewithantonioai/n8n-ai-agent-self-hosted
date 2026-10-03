# Lesson 5 · Give your agent tools

▶ [Watch this lesson](https://youtu.be/nRxDPfsSjk0?t=699) (starts at 11:39)

## Goal

Lesson five. Give your agent tools.

## In this lesson

Import [`app/workflows/02b-assistant-tools.json`](../../app/workflows/02b-assistant-tools.json): the same assistant with three tools. **Get weather** is an HTTP Request tool whose URL uses `{{ $fromAI('latitude', 'Latitude of the place', 'number') }}` and `{{ $fromAI('longitude', 'Longitude of the place', 'number') }}`; plus **Calculator** and **Wikipedia**.

## Recap

So: tools are functions the model can call. Dollar from AI lets it fill in the parameters. And the logs show you every step. Next, an agent that works without you.
