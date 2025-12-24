# Cart Hdr

Datatype for commerce microservice.

## GET /cart-hdr/list

List Cart Hdr by user_id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| userId | query | Yes | integer | user_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /cart-hdr/lookup

Lookup Cart Hdr

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cartToken | query | No | string | cart_token |
| contactId | query | Yes | integer | contact_id |
| customerId | query | Yes | integer | customer_id |
| userCartNo | query | No | integer | user_cart_no |
| userId | query | Yes | integer | user_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /cart-hdr/{cartHdrUid}/also-bought

List Also Bought data for Cart Hdr

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cart_hdr_uid | path | Yes | integer | cart_hdr_uid |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
