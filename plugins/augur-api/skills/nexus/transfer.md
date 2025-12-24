# Transfer

Datatype for nexus microservice.

## GET /transfer/{transferUid}

Get Transfer Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_uid | path | Yes | integer | transfer_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /transfer/{transferUid}

Update Transfer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_uid | path | Yes | integer | transfer_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /transfer/{transferUid}

DELETE Transfer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| transfer_uid | path | Yes | integer | transfer_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /transfer

List Transfers

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

## POST /transfer

Create Transfer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
