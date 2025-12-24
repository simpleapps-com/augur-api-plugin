---
name: Payments API
description: Use when working with element, health check, moneris, seed, unified, or making API calls to https://payments.augur-api.com.
version: 1.0.3
---

# Payments

Service-specific knowledge for payments microservice.

## API Documentation

- [OpenAPI Specification](https://payments.augur-api.com/openapi.json)
- [Postman Collection](https://payments.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### element

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /element/payment | Create payment account token from card data | [element.md](element.md#post-elementpayment) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### moneris

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /moneris/pre-auth-complete | Completes a pre-authorization transaction. | [moneris.md](moneris.md#get-monerispre-auth-complete) |
| GET | /moneris/pre-auth | Pre-authorizes a transaction. | [moneris.md](moneris.md#get-monerispre-auth) |

### unified

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /unified/account-query | Get account query with transaction setup id | [unified.md](unified.md#get-unifiedaccount-query) |
| GET | /unified/billing-update | Update billing information with transaction setup id | [unified.md](unified.md#get-unifiedbilling-update) |
| GET | /unified/card-info | Get card information with transaction setup id | [unified.md](unified.md#get-unifiedcard-info) |
| GET | /unified/surcharge | Get surcharge with payment account id | [unified.md](unified.md#get-unifiedsurcharge) |
| GET | /unified/transaction-setup | Create a transaction with customer and account information | [unified.md](unified.md#get-unifiedtransaction-setup) |
| GET | /unified/validate | Validate a transaction with customer and account information | [unified.md](unified.md#get-unifiedvalidate) |
