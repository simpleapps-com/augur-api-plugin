---
name: Agr Info API
description: Use when working with akasha, auggie, basecamp, basecamp threads, context, data type context, health check, joomla, memo, microservices, note, oauth, ollama, rubrics, seed, sites, workflows, or making API calls to https://agr-info.augur-api.com.
version: 1.0.5
---

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

### context

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /context/{siteId} | get the context for a site | [context.md](context.md#get-contextsiteId) |

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

### oauth

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /oauth/refresh | Rotate a refresh token; returns a new access/refresh pair | [oauth.md](oauth.md#post-oauthrefresh) |
| DELETE | /oauth/grants/{grantId} | Revoke a grant; idempotent per RFC 7009 spirit | [oauth.md](oauth.md#delete-oauthgrantsgrantId) |

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

### sites

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /sites/validate | Validate credentials and return P21 connection details | [sites.md](sites.md#post-sitesvalidate) |
| POST | /sites/verify-user | Verify a Joomla password and issue an agr-int OAuth grant | [sites.md](sites.md#post-sitesverify-user) |

### workflows

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /workflows/{workflowsUid} | Get Workflow Details | [workflows.md](workflows.md#get-workflowsworkflowsUid) |
| PUT | /workflows/{workflowsUid} | Update Workflow | [workflows.md](workflows.md#put-workflowsworkflowsUid) |
| DELETE | /workflows/{workflowsUid} | Delete Workflow | [workflows.md](workflows.md#delete-workflowsworkflowsUid) |
| GET | /workflows | List Workflows | [workflows.md](workflows.md#get-workflows) |
| POST | /workflows | Create Workflow | [workflows.md](workflows.md#post-workflows) |
