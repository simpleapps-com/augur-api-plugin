# Item Wishlist Line

Datatype for items microservice.

## GET /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid}

List items in a wishlist

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_wishlist_hdr_uid | path | Yes | integer | item_wishlist_hdr.item_wishlist_hdr_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid}

Create one more more item in a wishlist

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_wishlist_hdr_uid | path | Yes | integer | item_wishlist_hdr.item_wishlist_hdr_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid}/line/{itemWishlistLineUid}

Delete an item from a wishlist

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_wishlist_hdr_uid | path | Yes | integer | item_wishlist_hdr.item_wishlist_hdr_uid |
| item_wishlist_line_uid | path | Yes | integer | item_wishlist_line.item_wishlist_line_uid |
| users_id | path | Yes | integer | joomla.users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
