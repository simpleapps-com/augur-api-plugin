# Inv Profile Line

Datatype for vmi microservice.

## GET /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line/{invProfileLineUid}

Get Inventory Profile line Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| inv_profile_line_uid | path | Yes | integer | invProfileLineUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line/{invProfileLineUid}

Update Inventory Profile line

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| inv_profile_line_uid | path | Yes | integer | invProfileLineUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line/{invProfileLineUid}

DELETE Inventory Profile Line

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| inv_profile_line_uid | path | Yes | integer | invProfileLineUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line

List Inventory Profile Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | No | string | Search keywords field |
| statusCd | query | No | int | Filter by status code (700=DELETE, 704=ACTIVE, 705=INACTIVE) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line

Create Inventory Profile Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_profile_hdr_uid | path | Yes | integer | invProfileHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
