---
name: Slack API
description: Use when working with health check, seed, slack api, users, web hook, or making API calls to https://slack.augur-api.com.
version: 1.0.3
---

# Slack

Service-specific knowledge for slack microservice.

## API Documentation

- [OpenAPI Specification](https://slack.augur-api.com/openapi.json)
- [Postman Collection](https://slack.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### web_hook

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /web-hook | Web Hook | [web_hook.md](web_hook.md#post-web-hook) |
| GET | /web-hook/refresh | Web Hook refresh | [web_hook.md](web_hook.md#get-web-hookrefresh) |
