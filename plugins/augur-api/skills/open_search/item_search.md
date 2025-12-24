# Item Search

Datatype for open_search microservice.

## GET /item-search

Perform Item Search

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheSiteId | query | No | string | The SiteId to use for edge caching. (Default: none) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| classId5ExcludeList | query | No | string | list of inv_mast.class_id5 values to exclude (CSV) |
| classId5List | query | No | string | list of inv_mast.class_id5 values (CSV) |
| discontinuedAny | query | No | string | Filter by discontinued status [Y|N] |
| fields | query | No | string | list of fields to query (CSV) |
| filters | query | No | string | A JSON representation of the filters [{attributeUid:attributeValueUid}] |
| from | query | No | integer | return results starting FROM this index |
| itemCategoryUidList | query | No | string | CSV is itemCategoryUids to limit search results |
| jobNumbers | query | No | string | A CSV of job numbers to filter |
| operator | query | No | string | search operator [AND|OR] (Default: OR) |
| parentCategoryUid | query | No | int | item_category_uid as parent with all children included |
| q | query | Yes | string | search query |
| searchType | query | Yes | string | Type of search: [similarity|query] (Default: query) |
| size | query | No | integer | size of search results |
| sort | query | No | string | Sort by field|direction (e.g., price1|asc, price2|desc, item_id|asc) |
| sourceFieldsList | query | No | string | list of source_fields to return (CSV) |
| stockStatus | query | No | string | Filter by stock status [in_stock|out_of_stock] |
| tags | query | No | string | A CSV of tags to filter |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
