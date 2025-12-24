# Trans User

Datatype for p21_apis microservice.

## GET /trans-user/{usersUid}

Get User Details by User UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| userId | query | No | string | User ID |
| users_uid | path | Yes | integer | User UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /trans-user/{usersUid}

Update User by User UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| userId | query | No | string | User ID |
| users_uid | path | Yes | integer | User UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /trans-user/{usersUid}

Delete User by User UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| userId | query | No | string | User ID |
| users_uid | path | Yes | integer | User UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /trans-user

Create User

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
