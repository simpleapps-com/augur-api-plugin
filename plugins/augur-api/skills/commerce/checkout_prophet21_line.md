# Checkout Prophet21 Line

Datatype for commerce microservice.

## POST /checkout/{checkoutUid}/prophet21-hdr/{prophet21HdrUid}/prophet21-line

Add items to Prophet 21 checkout

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| checkout_uid | path | Yes | integer | checkoutUid |
| prophet21_hdr_uid | path | Yes | integer | prophet21HdrUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
