# Item Favorites

Datatype for items microservice.

## GET /item-favorites/{usersId}

List the item favorites for a user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /item-favorites/{usersId}

Create a new item favorite

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /item-favorites/{usersId}/{invMastUid}

Update an item favorite

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | joomla.users.id |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /item-favorites/{usersId}/{invMastUid}

Soft Delete an item from a user's favorites

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | joomla.users.id |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
