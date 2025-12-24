# Products

Datatype for vmi microservice.

## POST /distributors/{distributorsUid}/products

Create Product

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributors_uid | path | Yes | integer | userId |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /products/{productsUid}

Get Product Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| products_uid | path | Yes | integer | productsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /products/{productsUid}

Update Product

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| products_uid | path | Yes | integer | products_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /products/{productsUid}

DELETE Product

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| products_uid | path | Yes | integer | productsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /products/{productsUid}/enable

Enable/Disable/Delete Product

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| products_uid | path | Yes | integer | products_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /products/find

Find products and items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | integer | customer.customer_id |
| prefix | query | No | string | Product Id Prefix |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /products

List products

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | integer | customer.customer_id |
| distributorsUid | query | Yes | integer | distributorsUid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| prefix | query | No | string | Product Id Prefix |
| q | query | No | string | Query String |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
