# Transfer Shipping

Datatype for nexus microservice.

## GET /transfer-shipping/{transferReceiptUid}

Get Transfer Shipping Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_receipt_uid | path | Yes | integer | transfer_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /transfer-shipping/{transferReceiptUid}

Update Transfer Shipping

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_receipt_uid | path | Yes | integer | transfer_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /transfer-shipping/{transferReceiptUid}

DELETE Transfer Shipping

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_receipt_uid | path | Yes | integer | transfer_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /transfer-shipping

List Transfer Shippings

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

## POST /transfer-shipping

Create Transfer Shipping

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
