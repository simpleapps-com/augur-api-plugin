# Item Uom

Datatype for items microservice.

## GET /item-uom/{itemUomUid}

Get Item UOM Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_uom_uid | path | Yes | integer | item_uom_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /item-uom

List Item UOMs

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| createdSince | query | No | string | Filter records created since date (YYYY-MM-DD HH:MM:SS) |
| deleteFlag | query | No | string | Filter by delete flag (N=active, Y=deleted) |
| invMastUid | query | No | integer | Item ID (inv_mast_uid) |
| limit | query | No | int | Limit number of results (Default: 10) |
| modifiedSince | query | No | string | Filter records modified since date (YYYY-MM-DD HH:MM:SS) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: item_uom_uid|ASC) |
| unitOfMeasure | query | No | string | Unit of Measure filter |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
