# Lesson 3 · Your first workflow

▶ [Watch this lesson](https://youtu.be/nRxDPfsSjk0?t=375) (starts at 6:15)

## Goal

Lesson three. Your first workflow.

## In this lesson

Import [`app/workflows/01-weather-check.json`](../../app/workflows/01-weather-check.json): Manual Trigger → HTTP Request (Open-Meteo, no API key) → Edit Fields with the expressions `{{ $json.current.temperature_2m }}` and `{{ $json.current.wind_speed_10m }}`. Click **Execute workflow**.

## Recap

So: nodes pass items to each other. You execute a workflow to test it. And expressions read the data with dollar json. Now, let's add some intelligence.
