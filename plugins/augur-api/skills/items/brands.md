# Brands

Datatype for items microservice.

## GET /brands/{brandsUid}/attributes

List attributes for brand items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /brands/{brandsUid}

Get Brands Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brandsId | query | No | string | Brands ID for lookup when UID is 0 |
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
| orderBy | query | No | string | Order By (Default: brands_uid|ASC) |
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

## GET /brands/{brandsUid}/items

List items for a brand

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| brands_uid | path | Yes | integer | brands_uid |
| classId5ExcludeList | query | No | string | List of excluded class 5 values (default:blank) |
| classId5List | query | No | string | List of allowed class 5 values (default:blank) |
| displayOnWebFlag | query | No | string | Display on web flag [Y|N|Blank] (Default: Blank) |
| fields | query | No | string | fields to filter with (Default: itemId, itemDesc, ExtendedDesc) |
| filters | query | No | string | A JSON representation of the filters [{attributeUid:attributeValueUid}] |
| includeStock | query | No | string | Include Stock [Y|N] (Default: N) |
| limit | query | No | int | Limit number of results (Default: 12) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | No | string | search query (optional) |
| sortBy | query | No | string | Field from Document to sort by (Default: item_id) |
| tags | query | No | string | A CSV of tags |
| variantFilter | query | No | string | Filter variants [primary_only] (Default: blank) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
