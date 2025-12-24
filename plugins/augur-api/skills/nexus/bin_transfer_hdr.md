# Bin Transfer Hdr

Datatype for nexus microservice.

## GET /bin-transfer/{binTransferHdrUid}

Get Bin Transfer Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin_transfer_hdr_uid | path | Yes | integer | bin_transfer_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /bin-transfer/{binTransferHdrUid}

Update Bin Transfer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin_transfer_hdr_uid | path | Yes | integer | bin_transfer_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /bin-transfer/{binTransferHdrUid}

DELETE Bin Transfer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin_transfer_hdr_uid | path | Yes | integer | bin_transfer_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /bin-transfer

List Bin Transfers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /bin-transfer

Create Bin Transfer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /bin-transfer/{binTransferHdrUid}/status

Get Bin Transfer Status with Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| bin_transfer_hdr_uid | path | Yes | integer | bin_transfer_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
