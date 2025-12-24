---
name: Shipping API
description: Use when working with health check, rates, or making API calls to https://shipping.augur-api.com.
version: 1.0.5
---

# Shipping

Service-specific knowledge for shipping microservice.

## API Documentation

- [OpenAPI Specification](https://shipping.augur-api.com/openapi.json)
- [Postman Collection](https://shipping.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### rates

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /rates | Get Rates from POST | [rates.md](rates.md#post-rates) |
