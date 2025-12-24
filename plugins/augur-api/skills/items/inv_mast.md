# Inv Mast

Datatype for items microservice.

## GET /inv-mast/{invMastUid}

get the inv_mast details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv-mast-uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/lookup

Lookup InvMast by search query

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| onlineCd | query | No | int | Online Code (online_cd) [(704)|(705)|(700)] |
| orderBy | query | No | string | Order by field and direction (e.g., item_id|ASC) |
| q | query | Yes | string | Search query for item lookup |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast

List InvMast

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| itemCategoryUid | query | No | int | item_category_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| onlineCd | query | No | int | Online Code (online_cd) [(704)|(705)|(700)] |
| prefix | query | No | string | ItemId Prefix |
| q | query | No | string | Search query for items |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/doc

get the inv_mast document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| includePricing | query | No | string | Include invMast price 1-10 [Y|N] (Default: N) |
| inv-mast-uid | path | Yes | integer | inv_mast.inv_mast_uid |
| itemId | query | No | string | itemId. Used for lookup if invMastUid is zero |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /p21/inv-mast

List raw inv_mast P21 data

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| createdSince | query | No | string | Created since date (YYYY-MM-DD HH:MM:SS) |
| limit | query | No | int | Limit number of results |
| modifiedSince | query | No | string | Modified since date (YYYY-MM-DD HH:MM:SS) |
| offset | query | No | int | Offset for pagination |
| onlineCd | query | No | int | Online code filter (704/705/700) |
| orderBy | query | No | string | Order by field and direction (e.g., item_id|ASC) |
| statusCd | query | No | int | Status code filter (704/705/700) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
