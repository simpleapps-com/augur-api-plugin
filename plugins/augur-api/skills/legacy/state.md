# State

Datatype for legacy microservice.

## GET /legacy/state/{stateUid}

Get State Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| state_uid | path | Yes | integer | state_uid |
| twoLetterCode | query | No | string | State Abbreviation |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /legacy/state/{stateUid}

Update State

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| state_uid | path | Yes | integer | state_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /legacy/state/{stateUid}

DELETE State

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| state_uid | path | Yes | integer | state_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /legacy/state

List States

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| twoLetterCode | query | No | string | State Abbreviation |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /legacy/state

Create State

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
