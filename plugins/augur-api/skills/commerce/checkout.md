# Checkout

Datatype for commerce microservice.

## POST /checkout

Create new Checkout

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /checkout/{checkoutUid}

Get Checkout Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| checkout_uid | path | Yes | integer | checkoutUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /checkout/{checkoutUid}/activate

Activate Checkout

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| checkout_uid | path | Yes | integer | checkoutUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /checkout/{checkoutUid}/doc

Get Checkout Doc

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cartHdrUid | query | No | integer | cartHdrUid |
| checkout_uid | path | Yes | integer | checkoutUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /checkout/{checkoutUid}/validate

Validate Checkout

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| checkout_uid | path | Yes | integer | checkoutUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
