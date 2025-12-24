# Location

Datatype for p21_core microservice.

## GET /location/{locationId}

Get Location Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| location_id | path | Yes | number | location_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /location

List Locations

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| deleteFlag | query | No | string | Delete Flag |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: location_id|ASC) |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
