# Purchase Order Receipt

Datatype for nexus microservice.

## GET /purchase-order-receipt/{purchaseOrderReceiptUid}

Get Purchase Order Receipt Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| purchase_order_receipt_uid | path | Yes | integer | purchase_order_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /purchase-order-receipt/{purchaseOrderReceiptUid}

Update Purchase Order Receipt

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| purchase_order_receipt_uid | path | Yes | integer | purchase_order_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /purchase-order-receipt/{purchaseOrderReceiptUid}

DELETE Purchase Order Receipt

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| purchase_order_receipt_uid | path | Yes | integer | purchase_order_receipt_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /purchase-order-receipt

List Purchase Order Receipts

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

## POST /purchase-order-receipt

Create Purchase Order Receipt

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
