# People

Datatype for basecamp2 microservice.

## GET /people/{id}

Get Person by ID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Person ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /people

List People with filters

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| adminFlag | query | No | string | Filter by admin status (Y/N) |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset for results (Default: 0) |
| orderBy | query | No | string | Sort field (name, emailAddress) |
| q | query | No | string | Search name or emailAddress (LIKE) |
| trashedFlag | query | No | string | Filter by trashed status (Y/N) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /people/{personId}/projects/{projectId}/todos

List Todos for Person on Project

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| completedFlag | query | No | string | Filter by completion status (Y/N) |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: position|asc) |
| personId | path | Yes | integer | Person ID (assignee) |
| projectId | path | Yes | integer | Project ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /people/{id}/todos

List Todos for Person

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| completedFlag | query | No | string | Filter by completion status (Y/N) |
| dueAt | query | No | string | Filter by due date |
| id | path | Yes | integer | Person ID (assignee) |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: due_at|asc) |
| projectsId | query | No | integer | Filter by project ID (optional) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
