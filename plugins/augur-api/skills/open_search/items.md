# Items

Datatype for open_search microservice.

## PUT /items/refresh

refresh items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /items/{invMastUid}

get the item document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv-mast-uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /items/{invMastUid}

update the item document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv-mast-uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /items

List items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| itemId | query | No | string | Item ID prefix |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| online | query | No | string | Online status [Y|N] |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /items/{invMastUid}/refresh

refresh the item document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv-mast-uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
