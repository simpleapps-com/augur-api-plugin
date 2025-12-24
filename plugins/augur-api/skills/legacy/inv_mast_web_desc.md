# Inv Mast Web Desc

Datatype for legacy microservice.

## GET /inv-mast/{invMastUid}/web-desc/{invMastWebDescUid}

Get Item Web Description

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| inv_mast_web_desc_uid | path | Yes | integer | inv_mast_web_desc.inv_mast_web_desc_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /inv-mast/{invMastUid}/web-desc/{invMastWebDescUid}

Update Item Web Description

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| inv_mast_web_desc_uid | path | Yes | integer | inv_mast_web_desc.inv_mast_web_desc_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-mast/{invMastUid}/web-desc/{invMastWebDescUid}

Delete Item Web Description

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| inv_mast_web_desc_uid | path | Yes | integer | inv_mast_web_desc.inv_mast_web_desc_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/web-desc

List item Web Descriptions

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-mast/{invMastUid}/web-desc

Create Web Description for Item

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
