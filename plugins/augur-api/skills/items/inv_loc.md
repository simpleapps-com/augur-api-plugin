# Inv Loc

Datatype for items microservice.

## GET /inv-loc

List InvLoc

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| invMastUid | query | No | int | inv_mast_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/stock

get the inv_mast stock

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
