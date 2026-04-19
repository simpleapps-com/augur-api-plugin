# Item Variant Hdr X Attribute

Datatype for items microservice.

## GET /variants/{itemVariantHdrUid}/attributes/{attributeUid}

Get variant attribute link details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | attribute_uid |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /variants/{itemVariantHdrUid}/attributes/{attributeUid}

Update variant attribute link

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | attribute_uid |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /variants/{itemVariantHdrUid}/attributes/{attributeUid}

Remove attribute from variant

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| attribute_uid | path | Yes | integer | attribute_uid |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /variants/{itemVariantHdrUid}/attributes

List attributes for variant

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /variants/{itemVariantHdrUid}/attributes

Add attribute to variant

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
