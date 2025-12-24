# Unified

Datatype for payments microservice.

## GET /unified/account-query

Get account query with transaction setup id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | string | Customer ID for the transaction |
| mode | query | No | string | API mode for the transaction(Default: live|dev) |
| transactionSetupId | query | Yes | string | Transaction setup id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /unified/billing-update

Update billing information with transaction setup id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| address1 | query | Yes | string | Address 1 |
| address2 | query | No | string | Address 2 |
| city | query | Yes | string | City |
| mode | query | No | string | API mode for the transaction(Default: live|dev) |
| state | query | Yes | string | State |
| transactionSetupId | query | Yes | string | Transaction setup id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |
| zip | query | Yes | string | Zip |

---

## GET /unified/card-info

Get card information with transaction setup id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| mode | query | No | string | API mode for the transaction(Default: live|dev) |
| transactionSetupId | query | Yes | string | Transaction setup id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /unified/surcharge

Get surcharge with payment account id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| amount | query | Yes | string | Amount |
| country | query | Yes | string | Country |
| customerId | query | Yes | string | Customer ID for the transaction |
| fromState | query | Yes | string | From state |
| mode | query | No | string | API mode for the transaction(Default: live|dev) |
| paymentAccountId | query | Yes | string | Payment account id |
| toState | query | Yes | string | To state |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /unified/transaction-setup

Create a transaction with customer and account information

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | string | Customer ID for the transaction |
| mode | query | No | string | API mode for the transaction(dev or live) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /unified/validate

Validate a transaction with customer and account information

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | string | Customer ID for the transaction |
| mode | query | No | string | API mode for the transaction(Default: live|dev) |
| transactionSetupId | query | Yes | string | Transaction setup id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
