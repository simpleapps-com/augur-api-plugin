# Brands

Datatype for items microservice.

## GET /brands/{brandsUid}

Get Brands Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /brands/{brandsUid}

Update Brands

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /brands/{brandsUid}

DELETE Brands

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /brands

List Brands

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /brands

Create Brands

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
