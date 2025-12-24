# Inv Bin

Datatype for items microservice.

## GET /inv-mast/{invMastUid}/locations/{locationId}/bins/{bin}

Get a specific bin for an inventory item at a specific location

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin | path | Yes | string | bin identifier |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| location_id | path | Yes | integer | location.location_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/locations/{locationId}/bins

List bins for a specific location

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| excludeZero | query | No | string | Exclude bins with zero quantity [Y|N], defaults to Y |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| location_id | path | Yes | integer | location.location_id |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /locations/{locationId}/bins/{bin}

List all items in a specific bin

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin | path | Yes | string | bin identifier |
| excludeZero | query | No | string | Exclude bins with zero quantity [Y|N], defaults to Y |
| limit | query | No | int | Limit number of results (Default: 10) |
| location_id | path | Yes | integer | location.location_id |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /locations/{locationId}/bins

List all items in bins at a location

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin | query | No | string | bin identifier to filter by |
| excludeZero | query | No | string | Exclude bins with zero quantity [Y|N], defaults to Y |
| limit | query | No | int | Limit number of results (Default: 10) |
| location_id | path | Yes | integer | location.location_id |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
