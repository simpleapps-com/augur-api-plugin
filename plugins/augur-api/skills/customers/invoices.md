# Invoices

Datatype for customers microservice.

## GET /customer/{customerId}/invoices/{invoiceNo}

Get Customer Invoice

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| invoice_no | path | Yes | integer | invoice_hdr.invoice_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/{customerId}/invoices

List Customer Invoices

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| q | query | Yes | string | search query |
| shipToId | query | No | integer | invoice_hdr.ship_to_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
