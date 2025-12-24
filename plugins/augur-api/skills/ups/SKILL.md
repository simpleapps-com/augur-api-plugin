---
name: Ups API
description: Use when working with address validation, health check, rates, seed, ups oauth api, or making API calls to https://ups.augur-api.com.
version: 1.0.5
---

# Ups

Service-specific knowledge for ups microservice.

## API Documentation

- [OpenAPI Specification](https://ups.augur-api.com/openapi.json)
- [Postman Collection](https://ups.augur-api.com/postman.json)

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
| GET | /rates-shop | Shop UPS Rates | [rates.md](rates.md#get-rates-shop) |
