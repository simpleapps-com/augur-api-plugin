# Web Pricing

Datatype for pricing microservice.

## GET /web-pricing/{webPricingUid}

Get Web Pricing Rule

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| web_pricing_uid | path | Yes | integer | web_pricing_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /web-pricing

List Web Pricing Rules

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: web_pricing_uid|ASC) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
