---
type: service
id: llm-service
title: LLM Service
description: "AI language model provider for text analysis and summary generation"
tags: [Production]
connections: []
---

## Service

Provides access to a large language model for all text analysis, extraction, and synthesis tasks in the pipeline.

## Configuration

Connect this node to your preferred AI provider in the skrptiq app settings. Any capable language model will work. For longer books, a provider with a large context window (100k+ tokens) will produce better results during the synthesis stage.

## Supported Providers

- Anthropic Claude
- OpenAI GPT-4
- Google Gemini
- Any OpenAI-compatible API
