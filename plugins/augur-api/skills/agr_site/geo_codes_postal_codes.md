# Geo Codes Postal Codes

Datatype for agr_site microservice.

## GET /geo-codes-postal-codes/{geoCodesPostalCodesUid}

Get Postal Code Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| geo_codes_postal_codes_uid | path | Yes | integer | Postal Code UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /geo-codes-postal-codes

List Postal Codes

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: geo_codes_postal_codes_uid|ASC) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
