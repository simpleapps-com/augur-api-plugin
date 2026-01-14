# Comments

Datatype for basecamp2 microservice.

## GET /comments/{id}

Get Comment by ID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Comment ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /comments

List Comments

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| creatorId | query | No | integer | Filter by creator ID |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: id|asc) |
| todosId | query | No | integer | Filter by todos ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
