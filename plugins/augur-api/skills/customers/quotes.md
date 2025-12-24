# Quotes

Datatype for customers microservice.

## GET /customer/{customerId}/quotes/{quoteNo}

Get Customer Quote

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| quote_no | path | Yes | integer | quotes.quote_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/{customerId}/quotes

List Customer Quotes

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| orderBy | query | No | string | orderBy [date_created|DESC] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
