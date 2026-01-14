# Todos Sessions

Datatype for basecamp2 microservice.

## GET /todos/{id}/sessions

List Sessions for Todo

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| limit | query | No | int | Limit number of results (Default: 100) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Sort field (Default: session_num|desc) |
| sessionStatusCd | query | No | int | Filter by session status (100=open, 101=closed, 102=blocked) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /todos/{id}/sessions

Create Session for Todo

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /todos/{id}/sessions/{sessionId}

Get Session Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| sessionId | path | Yes | integer | Session UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /todos/{id}/sessions/{sessionId}

Update Session

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| sessionId | path | Yes | integer | Session UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /todos/{id}/sessions/{sessionId}

Delete Session

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo ID |
| sessionId | path | Yes | integer | Session UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
