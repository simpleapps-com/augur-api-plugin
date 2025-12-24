# Transfer Receipt

Datatype for nexus microservice.

## GET /transfer-receipt/{transferReceiptUid}

Get Transfer Receipt Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_receipt_uid | path | Yes | integer | transfer_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /transfer-receipt/{transferReceiptUid}

Update Transfer Receipt

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_receipt_uid | path | Yes | integer | transfer_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /transfer-receipt/{transferReceiptUid}

DELETE Transfer Receipt

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_receipt_uid | path | Yes | integer | transfer_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /transfer-receipt

List Transfer Receipts

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| referenceNo | query | No | string | Reference Number |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /transfer-receipt

Create Transfer Receipt

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
