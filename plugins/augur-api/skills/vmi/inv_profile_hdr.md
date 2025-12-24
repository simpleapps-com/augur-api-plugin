# Inv Profile Hdr

Datatype for vmi microservice.

## GET /inv-profile-hdr/{invProfileHdrUid}

Get Inventory Profile Header Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /inv-profile-hdr/{invProfileHdrUid}

Update Inventory Profile Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-profile-hdr/{invProfileHdrUid}

DELETE Inventory Profile Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-profile-hdr

List Inventory Profile Headers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | integer | Customer Id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-profile-hdr

Create Inventory Profile Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-profile-hdr/{customerId}/upload

Upload Excel file to create inventory profile headers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customerId |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
