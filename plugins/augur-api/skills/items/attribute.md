# Attribute

Datatype for items microservice.

## GET /attributes/{attributeUid}

Get Attribute Group Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | attribute_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /attributes/{attributeUid}

Update Attribute

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | attribute_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /attributes/{attributeUid}

DELETE Attribute

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | attribute_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /attributes

List Attributes

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: attribute_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|705|700] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /attributes

Create Attribute

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
