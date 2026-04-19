# Price Engine

Datatype for pricing microservice.

## GET /price-engine

Get Item Price

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheSiteId | query | No | string | The SiteId to use for edge caching. (Default: none) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| cartItems | query | No | string | Cart items for group break pricing (format: itemId:qty[:UOM],itemId:qty[:UOM]) |
| companyId | query | No | string | company_id |
| customerId | query | Yes | int | customer_id |
| itemId | query | Yes | string | item_id |
| quantity | query | No | int | quantity |
| shipToId | query | No | int | ship_to_id |
| unitOfMeasure | query | No | string | unit_of_measure |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /price-engine

Price multiple items with cart context for group break pricing

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
