# Item Favorites

Datatype for items microservice.

## GET /item-favorites/{usersId}/items

List the item favorites for a user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | integer | Number of results to return |
| offset | query | No | integer | Number of results to skip |
| orderBy | query | No | string | Order By (Default: item_favorites_uid|ASC) |
| useItemDoc | query | No | string | Return item doc data (Y/N) |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /item-favorites/{usersId}/items

Create item favorites

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /item-favorites/{usersId}/items/{invMastUid}

Get a single item favorite

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /item-favorites/{usersId}/items/{invMastUid}

Toggle an item favorite active/inactive

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /item-favorites/{usersId}/items/{invMastUid}

Soft Delete an item from a user's favorites

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
