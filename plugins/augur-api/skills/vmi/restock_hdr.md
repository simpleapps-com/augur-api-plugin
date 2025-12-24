# Restock Hdr

Datatype for vmi microservice.

## GET /restock-hdr/{restockHdrUid}

Get Restock Header Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| restock_hdr_uid | path | Yes | integer | restockHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /restock-hdr/{restockHdrUid}

Update Restock Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| restock_hdr_uid | path | Yes | integer | restockHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /restock-hdr/{restockHdrUid}

DELETE Restock Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| restock_hdr_uid | path | Yes | integer | restockHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /restock-hdr

List Restock Headers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributorsUid | query | No | integer | Filter by Distributor UID |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| warehouseUid | query | No | integer | Filter by Warehouse UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /restock-hdr

Create Restock Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
