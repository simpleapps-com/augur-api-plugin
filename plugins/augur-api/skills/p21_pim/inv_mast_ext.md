# Inv Mast Ext

Datatype for p21_pim microservice.

## GET /inv-mast-ext/{invMastExtUid}

Get Inv Mast Ext Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_ext_uid | path | Yes | integer | inv_mast_ext_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /inv-mast-ext/{invMastExtUid}

Update Inv Mast Ext

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_ext_uid | path | Yes | integer | inv_mast_ext_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-mast-ext/{invMastExtUid}

DELETE Inv Mast Ext

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_ext_uid | path | Yes | integer | inv_mast_ext_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast-ext

List Inv Mast Ext

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| invMastUid | query | No | integer | Inv Mast Uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: inv_mast_ext_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-mast-ext

Create Inv Mast Ext

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
