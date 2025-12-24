# Attribute X Attribute Group

Datatype for items microservice.

## GET /attribute-groups/{attributeGroupUid}/attributes/{attributeXAttributeGroupUid}

Get Attribute X Attribute Group Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| attribute_x_attribute_group_uid | path | Yes | integer | attribute_x_attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /attribute-groups/{attributeGroupUid}/attributes/{attributeXAttributeGroupUid}

Update Attribute X Attribute Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| attribute_x_attribute_group_uid | path | Yes | integer | attribute_x_attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /attribute-groups/{attributeGroupUid}/attributes/{attributeXAttributeGroupUid}

DELETE Attribute X Attribute Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| attribute_x_attribute_group_uid | path | Yes | integer | attribute_x_attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /attribute-groups/{attributeGroupUid}/attributes

List Attribute X Attribute Groups

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: attribute_x_attribute_group_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|705|700] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /attribute-groups/{attributeGroupUid}/attributes

Create Attribute X Attribute Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_group_uid | path | Yes | integer | attribute_group_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
