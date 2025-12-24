# Ship To

Datatype for customers microservice.

## GET /customer/{customerId}/ship-to

List Customer Ship-To Addresses

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

## GET /ship-to/refresh

Trigger a data refresh

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
