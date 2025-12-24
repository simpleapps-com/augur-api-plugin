# Categories

Datatype for items microservice.

## GET /categories/{itemCategoryUid}/attributes

list the attributes in a category

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| includeSubCategories | query | No | string | Include attributes from sub categories [Y|N] (Default: N) |
| item_category_uid | path | Yes | integer | item_category.item_category_uid |
| productCollection | query | No | string | Product Collection the category must be in. default: blank |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /categories/{itemCategoryUid}

Get the category details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| childrenFilter | query | No | string | Filter for children (Default: null) |
| childrenLimit | query | No | int | Limit number of results (Default: 0) |
| childrenOffset | query | No | int | Starting offset results (Default: 0) |
| classId5ExcludeList | query | No | string | List of excluded class 5 values (default:blank) |
| classId5List | query | No | string | List of allowed class 5 values (default:blank) |
| filters | query | No | string | A JSON representation of the filters [{attributeUid:attributeValueUid}] |
| item_category_uid | path | Yes | integer | item_category.item_category_uid |
| orderBy | query | No | string | Select order of the categories Default: item_category_desc|ASC |
| path | query | No | string | Path to lookup (Default: /) |
| productCollection | query | No | string | Product Collection the category must be in. default: blank |
| rootItemCategoryId | query | No | string | Root item_category.item_category_id (Default: ROOT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /categories/{itemCategoryUid}/images

list the images for a category

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| item_category_uid | path | Yes | integer | item_category.item_category_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /categories/{itemCategoryUid}/items

list the items in a category

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| classId5ExcludeList | query | No | string | List of excluded class 5 values (default:blank) |
| classId5List | query | No | string | List of allowed class 5 values (default:blank) |
| displayOnWebFlag | query | No | string | Display on web flag [Y|N|Blank] (Default: Blank) |
| fields | query | No | string | fields to filter with (Default: itemId, itemDesc, ExtendedDesc) |
| filters | query | No | string | A JSON representation of the filters [{attributeUid:attributeValueUid}] |
| includeStock | query | No | string | Include Stock [Y|N] (Default: N) |
| item_category_uid | path | Yes | integer | item_category.item_category_uid |
| jobNumbers | query | No | string | Job numbers (contracts) to filter items by - comma-separated |
| limit | query | No | int | Limit number of results (Default: 12) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | No | string | search query |
| sortBy | query | No | string | Field from Document to sort by (Default: item_id) |
| stockStatus | query | No | string | Filter by stock status [in_stock|out_of_stock] (Default: blank) |
| tags | query | No | string | A CSV of tags |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /categories/lookup

lookup the categories details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| path | query | No | string | Path to lookup (Default: /) |
| rootItemCategoryId | query | No | string | Root item_category.item_category_id (Default: ROOT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
