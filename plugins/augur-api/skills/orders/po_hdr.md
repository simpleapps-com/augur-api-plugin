# Po Hdr

Datatype for orders microservice.

## GET /po-hdr/{poNo}

get the purchase order details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| po_no | path | Yes | integer | po_hdr.po_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /po-hdr/{poNo}/doc

get the purchase order document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| po_no | path | Yes | integer | po_hdr.po_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /po-hdr

Lookup PoHdr

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| complete | query | No | string | complete status [Y|N|NULL] |
| limit | query | No | integer | limit |
| locationId | query | No | integer | location id |
| offset | query | No | integer | limit |
| q | query | No | string | search query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /po-hdr/scan

Scan for similar purchase orders based on criteria

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
