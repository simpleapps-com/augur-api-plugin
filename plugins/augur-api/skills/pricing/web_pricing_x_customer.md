# Web Pricing X Customer

Datatype for pricing microservice.

## GET /web-pricing/{webPricingUid}/customers/{customerId}

Get Web Pricing Customer

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | P21 customer ID |
| web_pricing_uid | path | Yes | integer | web_pricing_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /web-pricing/{webPricingUid}/customers

List Web Pricing Customers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: web_pricing_x_customer_uid|ASC) |
| web_pricing_uid | path | Yes | integer | web_pricing_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
