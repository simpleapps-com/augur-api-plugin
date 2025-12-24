# Orders

Datatype for customers microservice.

## GET /customer/{customerId}/orders/{orderNo}

Get Customer Order

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| order_no | path | Yes | integer | oe_hdr.order_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/{customerId}/orders

List Customer Orders

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| address_id | path | Yes | integer | oe_hdr.address_id |
| cancelFlag | query | No | string | cancel flag [Y|N] (default N) |
| customer_id | path | Yes | integer | oe_hdr.customer_id |
| deleteFlag | query | No | string | delete flag [Y|N] (default N) |
| fullDocument | query | No | string | fullDocument vs summary [Y|N] (default Y) |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| orderBy | query | No | string | orderBy [date_created|DESC] |
| q | query | No | string | query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
