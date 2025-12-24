# Todos

Datatype for basecamp2 microservice.

## GET /todos/{id}

Get Todo Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /todos

List Todos

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: id|ASC) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
