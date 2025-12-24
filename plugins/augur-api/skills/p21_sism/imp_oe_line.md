# Imp Oe Line

Datatype for p21_sism microservice.

## GET /imp_oe_line/{importUid}/{lineNo}

Get ImpOeLine Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | integer | import_uid |
| line_no | path | Yes | integer | line_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /imp_oe_line/{importUid}/{lineNo}

Update ImpOeLine

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | integer | import_uid |
| line_no | path | Yes | integer | line_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /imp_oe_line

List ImpOeLines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| importUid | query | No | integer | Import UID |
| itemId | query | No | string | Item ID |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: import_uid|ASC) |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
