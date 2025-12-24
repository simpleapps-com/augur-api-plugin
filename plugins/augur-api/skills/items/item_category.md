# Item Category

Datatype for items microservice.

## GET /item-category/{itemCategoryUid}

get the item_category details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_category_uid | path | Yes | integer | item_category.item_category_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /item-category/lookup

lookup the item_category details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| path | query | No | string | Path to lookup (Default: /) |
| rootItemCategoryId | query | No | string | Root item_category.item_category_id (Default: ROOT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /item-category

list of categories

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | integer | Maximum number of records to return (default: 10) |
| offset | query | No | integer | Number of records to skip (default: 0) |
| q | query | No | string | Search query for filtering categories by id or description |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /item-category/{itemCategoryUid}/doc

get the item_category document

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| item_category_uid | path | Yes | integer | item_category.item_category_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
