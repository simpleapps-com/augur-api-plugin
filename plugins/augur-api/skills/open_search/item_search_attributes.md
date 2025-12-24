# Item Search Attributes

Datatype for open_search microservice.

## GET /item-search/attributes

Get Attributes from Item Search

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cacheSiteId | query | No | string | The SiteId to use for edge caching. (Default: none) |
| cacheTtl | query | No | integer | TTL for caching. Zero mean no cache. (Default: 0) |
| filters | query | No | string | A JSON representation of the filters [{attributeUid:attributeValueUid}] |
| q | query | Yes | string | search query |
| searchType | query | Yes | string | Type of search: [similarity|query] (Default: query) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
