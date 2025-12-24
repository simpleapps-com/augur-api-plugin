# Rates

Datatype for ups microservice.

## GET /rates-shop

Shop UPS Rates

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheSiteId | query | No | string | The SiteId to use for edge caching. (Default: none) |
| fromAddress1 | query | No | string | From Address Line 1 |
| fromAddress2 | query | No | string | From Address Line 2 |
| fromAddress3 | query | No | string | From Address Line 3 |
| fromCity | query | No | string | From City |
| fromCountryCode | query | No | string | From Country Code |
| fromPostalCode | query | No | string | From Postal Code |
| fromStateProvinceCode | query | No | string | From State/Province Code |
| toAddress1 | query | No | string | To Address Line 1 |
| toAddress2 | query | No | string | To Address Line 2 |
| toAddress3 | query | No | string | To Address Line 3 |
| toCity | query | No | string | To City |
| toCountryCode | query | No | string | To Country Code |
| toPostalCode | query | No | string | To Postal Code |
| toStateProvinceCode | query | No | string | To State/Province Code |
| weight | query | No | integer | Weight |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
