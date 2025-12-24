# Checkout Prophet21 Hdr

Datatype for commerce microservice.

## POST /checkout/{checkoutUid}/prophet21-hdr

Create new P21 Checkout

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| checkout_uid | path | Yes | integer | checkoutUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
