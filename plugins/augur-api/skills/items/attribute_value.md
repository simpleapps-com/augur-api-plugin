# Attribute Value

Datatype for items microservice.

## GET /attributes/{attributeUid}/values/{attributeValueUid}

Get AttributeValue Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attributeUid | path | Yes | integer | attribute_uid |
| attribute_value_uid | path | Yes | integer | attribute_value_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /attributes/{attributeUid}/values/{attributeValueUid}

Update AttributeValue

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attributeUid | path | Yes | integer | attribute_uid |
| attribute_value_uid | path | Yes | integer | attribute_value_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /attributes/{attributeUid}/values/{attributeValueUid}

DELETE AttributeValue

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attributeUid | path | Yes | integer | attribute_uid |
| attribute_value_uid | path | Yes | integer | attribute_value_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /attributes/{attributeUid}/values

List AttributeValues

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attributeUid | path | Yes | integer | Attribute Uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: attribute_value_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /attributes/{attributeUid}/values

Create AttributeValue

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attributeUid | path | Yes | integer | Attribute Uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
