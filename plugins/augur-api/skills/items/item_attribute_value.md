# Item Attribute Value

Datatype for items microservice.

## PUT /inv-mast/{invMastUid}/attributes/{attributeUid}/values/{attributeValueUid}

Update the status of an attribute value

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | item_attribute.attribute_uid |
| attribute_value_uid | path | Yes | integer | item_attribute_value.attribute_value_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-mast/{invMastUid}/attributes/{attributeUid}/values/{attributeValueUid}

Soft delete an attribute value

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | item_attribute.attribute_uid |
| attribute_value_uid | path | Yes | integer | item_attribute_value.attribute_value_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/attributes/{attributeUid}/values

List values for a specific item attribute

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | item_attribute.attribute_uid |
| attributeValueUid | query | No | integer | item_attribute_value.attribute_value_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| limit | query | No | integer | Limit number of results (Default: 10) |
| offset | query | No | integer | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: item_attribute_value_uid|ASC) |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-mast/{invMastUid}/attributes/{attributeUid}/values

Create a new attribute value for an item using a specific attribute

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | item_attribute.attribute_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/attributes

List item attributes

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| limit | query | No | integer | Maximum number of records to return |
| offset | query | No | integer | Record number to start from |
| orderBy | query | No | string | Order By (Default: item_attribute_value_uid|ASC) |
| q | query | No | string | Filter attribute values |
| statusCd | query | No | integer | item_attribute_value.status_cd |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-mast/{invMastUid}/attributes

Create a new attribute value for an item

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
