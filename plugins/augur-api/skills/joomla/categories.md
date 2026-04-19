# Categories

Datatype for joomla microservice.

## GET /categories/{id}

Get Category by ID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | categories.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /categories

List Categories

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| extension | query | No | string | Extension filter (e.g. com_content) |
| limit | query | No | integer | Limit number of results (Default: 10) |
| offset | query | No | integer | Offset number of results (Default: 0) |
| orderBy | query | No | string | Sort ordering (Default: id|ASC) |
| parentId | query | No | integer | Parent category ID |
| published | query | No | integer | Published state filter |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
