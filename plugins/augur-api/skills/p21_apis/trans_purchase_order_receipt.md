# Trans Purchase Order Receipt

Datatype for p21_apis microservice.

## GET /trans-purchase-order-receipt/{poNo}

Get Purchase Order Receipt Details by PO Number

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| po_no | path | Yes | string | Purchase Order Number |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /trans-purchase-order-receipt/{poNo}

Update Purchase Order Receipt by PO Number

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| po_no | path | Yes | string | Purchase Order Number |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
