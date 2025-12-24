# Inv Mast Tags

Datatype for legacy microservice.

## GET /inv-mast/:invMastUid/tags/:invMastTagsUid

Get Inv Mast Tag Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_tags_uid | path | Yes | integer | inv_mast_tags_uid |
| inv_mast_uid | path | Yes | integer | inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /inv-mast/:invMastUid/tags/:invMastTagsUid

Update Inv Mast Tag

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_tags_uid | path | Yes | integer | inv_mast_tags_uid |
| inv_mast_uid | path | Yes | integer | inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-mast/:invMastUid/tags/:invMastTagsUid

Delete Inv Mast Tag

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_tags_uid | path | Yes | integer | inv_mast_tags_uid |
| inv_mast_uid | path | Yes | integer | inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/:invMastUid/tags

List Inv Mast Tags

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-mast/:invMastUid/tags

Create Inv Mast Tag

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
