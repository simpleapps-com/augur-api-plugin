# Basecamp2

Service-specific knowledge for basecamp2 microservice.

## API Documentation

- [OpenAPI Specification](https://basecamp2.augur-api.com/openapi.json)
- [Postman Collection](https://basecamp2.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### todos

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todos/{id} | Get Todo Details | [todos.md](todos.md#get-todosid) |
| GET | /todos | List Todos | [todos.md](todos.md#get-todos) |

### todos_summary

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todos-summary/{id} | Get Todo Summary Details | [todos_summary.md](todos_summary.md#get-todos-summaryid) |
| GET | /todos-summary | List Todo Summaries | [todos_summary.md](todos_summary.md#get-todos-summary) |
