# Tags

Datatype for joomla microservice.

## GET /tags

Get Tag List

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| catId | query | No | integer | catid |
| limit | query | No | integer | Limit number of results (Default: 12) |
| offset | query | No | integer | Offset number of results (Default: 0) |
| parentId | query | No | integer | parent_id |
| q | query | No | string | Query string |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
