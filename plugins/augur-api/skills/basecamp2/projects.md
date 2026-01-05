# Projects

Datatype for basecamp2 microservice.

## GET /projects/{id}

Get Project by ID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Project ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /projects

List Projects

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| archivedFlag | query | No | string | Filter by archived status (Y/N) |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: name|asc) |
| trashedFlag | query | No | string | Filter by trashed status (Y/N) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /projects/{id}/todos

List Todos for Project

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| assigneeId | query | No | integer | Filter by assignee (Person ID) |
| completedFlag | query | No | string | Filter by completion status (Y/N) |
| id | path | Yes | integer | Project ID |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: position|asc) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
