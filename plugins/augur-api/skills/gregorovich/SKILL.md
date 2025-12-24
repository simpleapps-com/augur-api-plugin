---
name: Gregorovich API
description: Use when working with agr info, agr site, chat gpt, documents, embeddings, gpt chat, groq, health check, inv mast context, items, ollama, open ai, prompts, rag data, seed, vector store, vllm, or making API calls to https://gregorovich.augur-api.com.
version: 1.0.3
---

# Gregorovich

Service-specific knowledge for gregorovich microservice.

## API Documentation

- [OpenAPI Specification](https://gregorovich.augur-api.com/openapi.json)
- [Postman Collection](https://gregorovich.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### chat_gpt

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /chat-gpt/ask | ChatGPT Ask | [chat_gpt.md](chat_gpt.md#get-chat-gptask) |

### documents

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /documents | list the documents | [documents.md](documents.md#get-documents) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### ollama

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /ollama/generate | Ollama Generate | [ollama.md](ollama.md#post-ollamagenerate) |
