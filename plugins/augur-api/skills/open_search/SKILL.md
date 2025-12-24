---
name: Open Search API
description: Use when working with health check, item search, item search attributes, item search meta, items, query string, query string analytics, query string redirect, search options, seed, suggestions, or making API calls to https://open-search.augur-api.com.
version: 1.0.5
---

# Open Search

Service-specific knowledge for open_search microservice.

## API Documentation

- [OpenAPI Specification](https://open-search.augur-api.com/openapi.json)
- [Postman Collection](https://open-search.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### item_search

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-search | Perform Item Search | [item_search.md](item_search.md#get-item-search) |

### item_search_attributes

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-search/attributes | Get Attributes from Item Search | [item_search_attributes.md](item_search_attributes.md#get-item-searchattributes) |

### items

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| PUT | /items/refresh | refresh items | [items.md](items.md#put-itemsrefresh) |
| GET | /items/{invMastUid} | get the item document | [items.md](items.md#get-itemsinvMastUid) |
| PUT | /items/{invMastUid} | update the item document | [items.md](items.md#put-itemsinvMastUid) |
| GET | /items | List items | [items.md](items.md#get-items) |
| GET | /items/{invMastUid}/refresh | refresh the item document | [items.md](items.md#get-itemsinvMastUidrefresh) |

### suggestions

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /suggestions/{suggestionsUid} | Get Suggestion Details | [suggestions.md](suggestions.md#get-suggestionssuggestionsUid) |
| GET | /suggestions | List Suggestions | [suggestions.md](suggestions.md#get-suggestions) |
| GET | /suggestions/suggest | Get search suggestions for autocomplete | [suggestions.md](suggestions.md#get-suggestionssuggest) |
