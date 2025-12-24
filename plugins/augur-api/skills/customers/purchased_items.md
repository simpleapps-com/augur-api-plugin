# Purchased Items

Datatype for customers microservice.

## GET /customer/{customerId}/purchased-items

List Customer Purchased Items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| orderBy | query | No | string | orderBy [date_last_purchased|DESC] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
