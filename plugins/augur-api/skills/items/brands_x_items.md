# Brands X Items

Datatype for items microservice.

## GET /brands/{brandsUid}/items/{brandsXItemsUid}

Get Brands X Items Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| brands_x_items_uid | path | Yes | integer | brands_x_items_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /brands/{brandsUid}/items/{brandsXItemsUid}

Update Brands X Items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| brands_x_items_uid | path | Yes | integer | brands_x_items_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /brands/{brandsUid}/items/{brandsXItemsUid}

DELETE Brands X Items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| brands_x_items_uid | path | Yes | integer | brands_x_items_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /brands/{brandsUid}/items

List Brands X Items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /brands/{brandsUid}/items

Create Brands X Items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
