# Oe Hdr

Datatype for orders microservice.

## GET /oe-hdr/lookup

Lookup OeHdr summary

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| class1Id | query | No | string | taker |
| completed | query | No | string | completed |
| dateOrderCompleted | query | No | string | date_order_completed |
| limit | query | No | integer | limit |
| offset | query | No | integer | limit |
| orderBy | query | No | string | taker |
| q | query | No | string | query |
| salesrepId | query | No | string | salesrep_id |
| taker | query | No | string | taker |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /oe-hdr/{orderNo}/doc

get the order document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| order_no | path | Yes | integer | oe_hdr.order_no |
| postalCode | query | No | string | postal code |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
