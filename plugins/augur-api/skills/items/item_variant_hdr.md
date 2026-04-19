# Item Variant Hdr

Datatype for items microservice.

## GET /variants/{itemVariantHdrUid}

Get Item Variant Header Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /variants/{itemVariantHdrUid}

Update Item Variant Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /variants/{itemVariantHdrUid}

DELETE Item Variant Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /variants/{itemVariantHdrUid}/doc

Get Variant Doc

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| itemId | query | No | string | Item ID for lookup when itemVariantHdrUid is 0 |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid (use 0 with itemId query param for lookup) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /variants

List Item Variant Headers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: item_variant_hdr_uid|ASC) |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /variants

Create Item Variant Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /variants/{itemVariantHdrUid}/similar

Find Similar Items for Variant Header

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_variant_hdr_uid | path | Yes | integer | item_variant_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
