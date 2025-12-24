# Inv Warehouse

Datatype for vmi microservice.

## POST /warehouse/{warehouseUid}/adjust

Adjust Inventory

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /warehouse/{warehouseUid}/availability

List inventory availability

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| q | query | Yes | string | search query |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /warehouse/{warehouseUid}/receive

Receive Inventory

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /warehouse/{warehouseUid}/replenish

Get Replenish Information

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributorsUid | query | No | integer | distributors.distributors_uid |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /warehouse/{warehouseUid}/replenish

Replenish Inventory

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /warehouse/{warehouseUid}/transfer

Transfer Inventory

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouseUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
