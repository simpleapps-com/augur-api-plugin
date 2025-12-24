# Users

Datatype for joomla microservice.

## GET /users/{id}

Get User Detail

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /users/{id}

Update user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /users/{id}

BLOCK user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /users/{id}/doc

Get User Doc

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /users/{id}/trinity

Get Trinity User Doc

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| limit | query | No | integer | Limit number of results (Default: 10) |
| offset | query | No | integer | Offset number of results (Default: 0) |
| orderBy | query | No | string | Sort ordering: default (ordering|ASC) |
| q | query | No | string | Query string |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /users

Get User List

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /users

Create a user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| accessLevelList | query | No | string | CSV of Access Level IDs |
| customerId | query | No | integer | Customer ID |
| limit | query | No | integer | Limit number of results (Default: 10) |
| offset | query | No | integer | Offset number of results (Default: 0) |
| orderBy | query | No | string | orderBy |
| q | query | No | string | Query string |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /users/verify-password

Verify the password for a user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
