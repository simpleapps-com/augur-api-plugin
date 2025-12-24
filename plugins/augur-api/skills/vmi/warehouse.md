# Warehouse

Datatype for vmi microservice.

## GET /warehouse/{warehouseUid}

Get Warehouse Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /warehouse/{warehouseUid}

Update Warehouse

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /warehouse/{warehouseUid}

DELETE Warehouse

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /warehouse/{warehouseUid}/enable

Enable/Disable/Delete Warehouse

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /warehouse

List Warehouses

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | integer | Customer Id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: warehouse_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| usersId | query | No | int | Users Id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /warehouse

Create Warehouse

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
