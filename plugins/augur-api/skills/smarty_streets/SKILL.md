---
name: Smarty Streets API
description: Use when working with health check, seed, street, or making API calls to https://smarty-streets.augur-api.com.
version: 1.0.2
---

# Smarty Streets

Service-specific knowledge for smarty_streets microservice.

## API Documentation

- [OpenAPI Specification](https://smarty-streets.augur-api.com/openapi.json)
- [Postman Collection](https://smarty-streets.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### street

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /us/lookup | Lookup US Address | [street.md](street.md#get-uslookup) |
