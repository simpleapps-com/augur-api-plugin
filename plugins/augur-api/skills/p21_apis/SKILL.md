---
name: P21 Apis API
description: Use when working with common, data elements, document, entity addresses, entity contacts, entity customers, extensibility user defined fields, health check, interactive, inventory, rest api, rest inventory movement, rest inventory parts price, security token, seed, service definition, trans bin adjustment, trans bin inventory movement, trans bin location, trans bin type, trans category, trans class maintenance, trans company, trans customer, trans cycle count location criteria, trans item, trans order, trans purchase order, trans purchase order receipt, trans transfer, trans transfer receipt, trans transfer shipping, trans user, trans web display type, transactional api, or making API calls to https://p21-apis.augur-api.com.
version: 1.0.2
---

# P21 Apis

Service-specific knowledge for p21_apis microservice.

## API Documentation

- [OpenAPI Specification](https://p21-apis.augur-api.com/openapi.json)
- [Postman Collection](https://p21-apis.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### entity_contacts

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /entity-contacts/refresh | Trigger a data refresh | [entity_contacts.md](entity_contacts.md#get-entity-contactsrefresh) |

### entity_customers

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /entity-customers/refresh | Trigger a data refresh | [entity_customers.md](entity_customers.md#get-entity-customersrefresh) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### trans_category

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /trans-category/{categoryUid} | Get Category Details by Category UID | [trans_category.md](trans_category.md#get-trans-categorycategoryUid) |
| PUT | /trans-category/{categoryUid} | Update Category by Category UID | [trans_category.md](trans_category.md#put-trans-categorycategoryUid) |
| DELETE | /trans-category/{categoryUid} | Delete Category by Category UID | [trans_category.md](trans_category.md#delete-trans-categorycategoryUid) |
| POST | /trans-category | Create Category | [trans_category.md](trans_category.md#post-trans-category) |

### trans_company

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /trans-company/{companyUid} | Get Company Details by Company UID | [trans_company.md](trans_company.md#get-trans-companycompanyUid) |
| PUT | /trans-company/{companyUid} | Update Company by Company UID | [trans_company.md](trans_company.md#put-trans-companycompanyUid) |
| DELETE | /trans-company/{companyUid} | Delete Company by Company UID | [trans_company.md](trans_company.md#delete-trans-companycompanyUid) |
| POST | /trans-company | Create Company | [trans_company.md](trans_company.md#post-trans-company) |

### trans_purchase_order_receipt

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /trans-purchase-order-receipt/{poNo} | Get Purchase Order Receipt Details by PO Number | [trans_purchase_order_receipt.md](trans_purchase_order_receipt.md#get-trans-purchase-order-receiptpoNo) |
| PUT | /trans-purchase-order-receipt/{poNo} | Update Purchase Order Receipt by PO Number | [trans_purchase_order_receipt.md](trans_purchase_order_receipt.md#put-trans-purchase-order-receiptpoNo) |

### trans_user

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /trans-user/{usersUid} | Get User Details by User UID | [trans_user.md](trans_user.md#get-trans-userusersUid) |
| PUT | /trans-user/{usersUid} | Update User by User UID | [trans_user.md](trans_user.md#put-trans-userusersUid) |
| DELETE | /trans-user/{usersUid} | Delete User by User UID | [trans_user.md](trans_user.md#delete-trans-userusersUid) |
| POST | /trans-user | Create User | [trans_user.md](trans_user.md#post-trans-user) |

### trans_web_display_type

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /trans-web-display-type/{webDisplayTypeUid} | Get Web Display Type Details by Display Type UID | [trans_web_display_type.md](trans_web_display_type.md#get-trans-web-display-typewebDisplayTypeUid) |
| PUT | /trans-web-display-type/{webDisplayTypeUid} | Update Web Display Type by Display Type UID | [trans_web_display_type.md](trans_web_display_type.md#put-trans-web-display-typewebDisplayTypeUid) |
| DELETE | /trans-web-display-type/{webDisplayTypeUid} | Delete Web Display Type by Display Type UID | [trans_web_display_type.md](trans_web_display_type.md#delete-trans-web-display-typewebDisplayTypeUid) |
| GET | /trans-web-display-type/defaults | Get Web Display Type Defaults | [trans_web_display_type.md](trans_web_display_type.md#get-trans-web-display-typedefaults) |
| GET | /trans-web-display-type/definition | Get Web Display Type Definition | [trans_web_display_type.md](trans_web_display_type.md#get-trans-web-display-typedefinition) |
| POST | /trans-web-display-type | Create Web Display Type | [trans_web_display_type.md](trans_web_display_type.md#post-trans-web-display-type) |
