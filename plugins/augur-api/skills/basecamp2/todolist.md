# Todolist

Datatype for basecamp2 microservice.

## GET /todolists/{id}

Get Todolist Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todolist ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /todolists

List Todolists

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| assigneeId | query | No | integer | Filter by assignee ID |
| completedFlag | query | No | string | Filter by completion status (Y/N) |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: id|asc) |
| projectsId | query | No | integer | Filter by project ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
