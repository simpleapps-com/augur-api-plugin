# Agr Work

Service-specific knowledge for agr_work microservice.

## API Documentation

- [OpenAPI Specification](https://agr-work.augur-api.com/openapi.json)
- [Postman Collection](https://agr-work.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |
