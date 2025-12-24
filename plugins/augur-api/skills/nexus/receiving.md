# Receiving

Datatype for nexus microservice.

## GET /receiving/{receivingUid}

Get Receiving Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| receiving_uid | path | Yes | integer | receiving_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /receiving/{receivingUid}

Update Receiving

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| receiving_uid | path | Yes | integer | receiving_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /receiving/{receivingUid}

DELETE Receiving

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| receiving_uid | path | Yes | integer | receiving_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /receiving

List Receiving Records

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| poNo | query | No | integer | PO Number |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /receiving

Create Receiving

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
