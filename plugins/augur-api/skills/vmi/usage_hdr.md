# Usage Hdr

Datatype for vmi microservice.

## POST /warehouse/{warehouseUid}/usage

Use Inventory

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
