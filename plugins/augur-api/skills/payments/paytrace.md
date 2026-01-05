# Paytrace

Datatype for payments microservice.

## POST /paytrace/authorization

Authorize a credit card transaction (pre-auth).

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | body | Yes | number | Dollar amount of the transaction |
| billing_address | body | No | object | Billing address object |
| credit_card | body | Yes | object | Credit card object with number, expiration_month, expiration_year |
| csc | body | No | string | Card security code (3-4 digits) |
| invoice_id | body | No | string | Invoice identifier |
| test_mode | body | No | boolean | Use sandbox mode (default: false) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /paytrace/capture

Capture a previously authorized transaction.

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | body | No | number | Amount to capture (optional, defaults to full amount) |
| test_mode | body | No | boolean | Use sandbox mode (default: false) |
| transaction_id | body | Yes | string | Transaction ID from authorization |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /paytrace/refund

Refund a settled transaction.

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | body | No | number | Amount to refund (optional, defaults to full amount) |
| test_mode | body | No | boolean | Use sandbox mode (default: false) |
| transaction_id | body | Yes | string | Transaction ID to refund |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /paytrace/sale

Process a sale transaction (authorize and capture).

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | body | Yes | number | Dollar amount of the transaction |
| billing_address | body | No | object | Billing address object |
| credit_card | body | Yes | object | Credit card object with number, expiration_month, expiration_year |
| csc | body | No | string | Card security code (3-4 digits) |
| invoice_id | body | No | string | Invoice identifier |
| test_mode | body | No | boolean | Use sandbox mode (default: false) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /paytrace/void

Void a pending transaction.

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| test_mode | body | No | boolean | Use sandbox mode (default: false) |
| transaction_id | body | Yes | string | Transaction ID to void |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
