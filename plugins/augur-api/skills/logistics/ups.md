# Ups

Datatype for logistics microservice.

## GET /ups/rates

Get UPS Shipping Rates

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| fromAddress1 | query | Yes | string | From address line 1 |
| fromCity | query | Yes | string | From city |
| fromCountryCode | query | No | string | From country code (default: US) |
| fromPostalCode | query | Yes | string | From postal code |
| fromStateProvinceCode | query | Yes | string | From state/province code |
| toAddress1 | query | Yes | string | To address line 1 |
| toCity | query | Yes | string | To city |
| toCountryCode | query | No | string | To country code (default: US) |
| toPostalCode | query | Yes | string | To postal code |
| toStateProvinceCode | query | Yes | string | To state/province code |
| weight | query | Yes | integer | Package weight in pounds |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
