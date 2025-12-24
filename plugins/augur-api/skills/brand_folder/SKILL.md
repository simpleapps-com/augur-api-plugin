# Brand Folder

Service-specific knowledge for brand_folder microservice.

## API Documentation

- [OpenAPI Specification](https://brand-folder.augur-api.com/openapi.json)
- [Postman Collection](https://brand-folder.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### categories

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /categories/focus | Set Category Focus | [categories.md](categories.md#post-categoriesfocus) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
