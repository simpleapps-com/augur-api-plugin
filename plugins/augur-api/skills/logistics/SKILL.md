---
name: Logistics API
description: Use when working with health check, seed, shipvia, speedship, or making API calls to https://logistics.augur-api.com.
version: 1.0.4
---

# Logistics

Service-specific knowledge for logistics microservice.

## API Documentation

- [OpenAPI Specification](https://logistics.augur-api.com/openapi.json)
- [Postman Collection](https://logistics.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### shipvia

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /shipvia/rates | Get ShipVia shipping rates from multiple carriers | [shipvia.md](shipvia.md#get-shipviarates) |
| GET | /shipvia/rates/ltl | Get ShipVia LTL (Less-Than-Truckload) freight rates from multiple carriers | [shipvia.md](shipvia.md#get-shipviaratesltl) |

### speedship

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /speedship/freight | Get Speedship Freight | [speedship.md](speedship.md#get-speedshipfreight) |
