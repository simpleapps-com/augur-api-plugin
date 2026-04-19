# Postal Codes X Shiptos

Datatype for agr_site microservice.

## GET /postal-codes-x-shiptos/{postalCodesXShiptosUid}

Get Postal Code X Ship To Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| postal_codes_x_shiptos_uid | path | Yes | integer | postalCodesXShiptosUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /postal-codes-x-shiptos/{postalCodesXShiptosUid}

Update Postal Code X Ship To

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| postal_codes_x_shiptos_uid | path | Yes | integer | postalCodesXShiptosUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /postal-codes-x-shiptos/{postalCodesXShiptosUid}

Soft Delete Postal Code X Ship To

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| postal_codes_x_shiptos_uid | path | Yes | integer | postalCodesXShiptosUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /postal-codes-x-shiptos

List Postal Codes X Ship Tos

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: postal_codes_x_shiptos_uid|ASC) |
| q | query | No | string | Search by postal code |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /postal-codes-x-shiptos

Create Postal Code X Ship To

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
