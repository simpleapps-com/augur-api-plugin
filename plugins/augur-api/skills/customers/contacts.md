# Contacts

Datatype for customers microservice.

## GET /contacts/{id}/customers

List Salesrep Customers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| class5Id | query | No | string | customer.class_5id (default: none) |
| id | path | Yes | integer | contacts.id |
| limit | query | No | integer | limit (default 10) |
| offset | query | No | integer | offset (default 0) |
| q | query | No | string | query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /contacts/{id}/doc

get the contact document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | contacts.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /contacts/{id}/web-allowance

Get the web allowance for a contact_id (USCCO)

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | contacts.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /contacts/refresh

Trigger a data refresh

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
