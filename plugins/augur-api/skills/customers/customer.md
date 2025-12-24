# Customer

Datatype for customers microservice.

## GET /customer/{customerId}/address

Lookup Customer Addresses

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| q | query | Yes | string | search query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/{customerId}/contacts

Lookup Customer Contacts

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| q | query | Yes | string | search query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /customer/{customerId}/contacts

Create new contact for customer_id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/{customerId}/doc

get the customer document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/{customerId}/ship-to

Lookup Customer ShipTo

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| q | query | Yes | string | search query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /customer/{customerId}/ship-to

Create new ship_to for customer_id

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer.customer_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer

list the customer documents

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| class5Id | query | No | string | customer.class_5id (default: none) |
| limit | query | No | integer | Limit number of results (Default: 10) |
| offset | query | No | integer | Offset number of results (Default: 0) |
| orderBy | query | No | string | Sort ordering: default (ordering|ASC) |
| q | query | No | string | Query string |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customer/lookup

Lookup Customer summary

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| q | query | Yes | string | search query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
