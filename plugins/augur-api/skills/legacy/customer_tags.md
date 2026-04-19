# Customer Tags

Datatype for legacy microservice.

## GET /customers/{customerId}/tags/{customerTagsUid}

Get Customer Tag Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer_id |
| customer_tags_uid | path | Yes | integer | customer_tags_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /customers/{customerId}/tags/{customerTagsUid}

Update Customer Tag

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer_id |
| customer_tags_uid | path | Yes | integer | customer_tags_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /customers/{customerId}/tags/{customerTagsUid}

Delete Customer Tag

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer_id |
| customer_tags_uid | path | Yes | integer | customer_tags_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /customers/{customerId}/tags

List Customer Tags

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customer_id | path | Yes | integer | customer_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /customers/{customerId}/tags

Create Customer Tag

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
