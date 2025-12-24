# Attribute Group

Datatype for items microservice.

## GET /attribute-groups/{attributeGroupUid}

Get Attribute Group Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /attribute-groups/{attributeGroupUid}

Update Attribute Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /attribute-groups/{attributeGroupUid}

DELETE Attribute Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /attribute-groups

List Attribute Groups

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: attribute_group_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|705|700] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /attribute-groups

Create Attribute Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
