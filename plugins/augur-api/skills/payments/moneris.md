# Moneris

Datatype for payments microservice.

## GET /moneris/pre-auth-complete

Completes a pre-authorization transaction.

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | query | Yes | number | Amount of the transaction |
| orderId | query | Yes | string | Order ID for the transaction |
| testMode | query | No | boolean | API mode for the transaction(Default: true) |
| txnNumber | query | Yes | string | Transaction number |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /moneris/pre-auth

Pre-authorizes a transaction.

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | query | Yes | number | Amount of the transaction |
| ccNumber | query | Yes | string | credit card number |
| expDate | query | Yes | string | expiration date of the credit card(YYMM) |
| orderId | query | Yes | string | Order ID for the transaction |
| testMode | query | No | boolean | Test mode for the transaction(Default: false) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
