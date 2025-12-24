# Settings

Datatype for agr_site microservice.

## GET /settings/{settingsUid}

Get Settings Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| settings_uid | path | Yes | integer | settings_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /settings/{settingsUid}

Update Settings

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| settings_uid | path | Yes | integer | settings_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /settings/{settingsUid}

DELETE Settings

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| settings_uid | path | Yes | integer | settings_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /settings

List Settings

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| serviceName | query | Yes | string | Service Name |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /settings

Create Settings

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
