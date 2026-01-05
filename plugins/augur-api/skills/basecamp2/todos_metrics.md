# Todos Metrics

Datatype for basecamp2 microservice.

## GET /people/{id}/metrics

List Todo Metrics by Person

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| hasComments | query | No | integer | Filter by has comments (1=yes) |
| id | path | Yes | integer | Person ID (assignee) |
| isStale | query | No | integer | Filter stale todos (1=stale) |
| limit | query | No | integer | Limit number of results (Default: 100) |
| needsResponse | query | No | integer | Filter needs response (1=yes) |
| offset | query | No | integer | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: id|ASC) |
| todosStatusCd | query | No | integer | Filter by status (1=open, 2=completed) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /projects/{id}/metrics

List Todo Metrics by Project

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| hasComments | query | No | integer | Filter by has comments (1=yes) |
| id | path | Yes | integer | Project ID |
| isStale | query | No | integer | Filter stale todos (1=stale) |
| limit | query | No | integer | Limit number of results (Default: 100) |
| needsResponse | query | No | integer | Filter needs response (1=yes) |
| offset | query | No | integer | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: id|ASC) |
| todosStatusCd | query | No | integer | Filter by status (1=open, 2=completed) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /todos/{id}/metrics

Get Todo Metrics Detail

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /metrics

List Todo Metrics

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| assigneeId | query | No | integer | Filter by assignee ID |
| creatorId | query | No | integer | Filter by creator ID |
| hasComments | query | No | integer | Filter by has comments (1=yes) |
| isStale | query | No | integer | Filter stale todos (1=stale) |
| limit | query | No | integer | Limit number of results (Default: 100) |
| needsResponse | query | No | integer | Filter needs response (1=yes) |
| offset | query | No | integer | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: id|ASC) |
| projectsId | query | No | integer | Filter by project ID |
| todosStatusCd | query | No | integer | Filter by status (1=open, 2=completed) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
