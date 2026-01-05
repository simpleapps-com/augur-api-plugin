# Todos Events

Datatype for basecamp2 microservice.

## GET /todos/{id}/events

List Events for a Todo

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| eventTypeCd | query | No | int | Filter by event type (1=created, 2=comment, 3=completed) |
| id | path | Yes | integer | Todos ID |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: event_at|desc) |
| peopleId | query | No | integer | Filter by person ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /todos/{id}/events/{eventNum}

Get Todo Event Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| event_num | path | Yes | integer | Event sequence number (0=created, 1+=comments) |
| id | path | Yes | integer | Todos ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /events

List Todo Events

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| eventTypeCd | query | No | int | Filter by event type (1=created, 2=comment, 3=completed) |
| id | query | No | integer | Filter by todos ID |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: event_at|desc) |
| peopleId | query | No | integer | Filter by person ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
