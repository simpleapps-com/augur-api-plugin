# Item Variant Line

Datatype for items microservice.

## GET /variants/{itemVariantHdrUid}/lines/{itemVariantLineUid}

Get Item Variant Line Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | itemVariantHdrUid |
| item_variant_line_uid | path | Yes | integer | itemVariantLineUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /variants/{itemVariantHdrUid}/lines/{itemVariantLineUid}

Update Item Variant Line

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | itemVariantHdrUid |
| item_variant_line_uid | path | Yes | integer | itemVariantLineUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /variants/{itemVariantHdrUid}/lines/{itemVariantLineUid}

DELETE Item Variant Line

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | itemVariantHdrUid |
| item_variant_line_uid | path | Yes | integer | itemVariantLineUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /variants/{itemVariantHdrUid}/lines

List Item Variant Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | itemVariantHdrUid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /variants/{itemVariantHdrUid}/lines

Create Item Variant Line

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | itemVariantHdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
