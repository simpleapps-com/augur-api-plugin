# Avalara

Service-specific knowledge for avalara microservice.

## API Documentation

- [OpenAPI Specification](https://avalara.augur-api.com/openapi.json)
- [Postman Collection](https://avalara.augur-api.com/postman.json)

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
