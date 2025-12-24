# Item Wishlist Hdr

Datatype for items microservice.

## GET /item-wishlist/{usersId}

List the item wishlists for a user

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /item-wishlist/{usersId}

Create a new item wishlist

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid}

Update a new item wishlist

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_wishlist_hdr_uid | path | Yes | integer | item_wishlist_hdr.item_wishlist_hdr_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid}

Delete an item wishlist

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_wishlist_hdr_uid | path | Yes | integer | item_wishlist_hdr.item_wishlist_hdr_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
