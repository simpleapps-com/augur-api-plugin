# Agr Info

Service-specific knowledge for agr_info microservice.

## API Documentation

- [OpenAPI Specification](https://agr-info.augur-api.com/openapi.json)
- [Postman Collection](https://agr-info.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### akasha

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /akasha/generate | Generate Response from akasha | [akasha.md](akasha.md#post-akashagenerate) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### joomla

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /joomla/generate | Generate Response from joomla | [joomla.md](joomla.md#post-joomlagenerate) |

### microservices

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /microservices/{microservicesUid} | Get Microservice Details | [microservices.md](microservices.md#get-microservicesmicroservicesUid) |
| PUT | /microservices/{microservicesUid} | Update Microservice | [microservices.md](microservices.md#put-microservicesmicroservicesUid) |
| DELETE | /microservices/{microservicesUid} | DELETE Microservice | [microservices.md](microservices.md#delete-microservicesmicroservicesUid) |
| GET | /microservices | List Microservices | [microservices.md](microservices.md#get-microservices) |
| POST | /microservices | Create Microservice | [microservices.md](microservices.md#post-microservices) |

### ollama

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /ollama/tags | Get a list of tags/models | [ollama.md](ollama.md#get-ollamatags) |

### rubrics

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /rubrics/{rubricsUid} | Get Rubric Details | [rubrics.md](rubrics.md#get-rubricsrubricsUid) |
| PUT | /rubrics/{rubricsUid} | Update Rubric | [rubrics.md](rubrics.md#put-rubricsrubricsUid) |
| DELETE | /rubrics/{rubricsUid} | Delete Rubric | [rubrics.md](rubrics.md#delete-rubricsrubricsUid) |
| GET | /rubrics | List Rubrics | [rubrics.md](rubrics.md#get-rubrics) |
| POST | /rubrics | Create Rubric | [rubrics.md](rubrics.md#post-rubrics) |
