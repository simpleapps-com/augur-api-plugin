# Orders

Datatype for legacy microservice.

## GET /orders/{id}/reset

Reset orders for processing by id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | orders:id, web_orders_uid; web_reference_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
