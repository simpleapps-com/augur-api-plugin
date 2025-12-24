# Trans Category

Datatype for p21_apis microservice.

## GET /trans-category/{categoryUid}

Get Category Details by Category UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| categoryId | query | No | string | Category ID |
| category_uid | path | Yes | integer | Category UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /trans-category/{categoryUid}

Update Category by Category UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| categoryId | query | No | string | Category ID |
| category_uid | path | Yes | integer | Category UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /trans-category/{categoryUid}

Delete Category by Category UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| categoryId | query | No | string | Category ID |
| category_uid | path | Yes | integer | Category UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /trans-category

Create Category

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
