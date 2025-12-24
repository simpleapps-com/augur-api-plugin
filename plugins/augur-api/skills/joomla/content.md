# Content

Datatype for joomla microservice.

## GET /content/{id}

Get Content Detail

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| alias | query | No | string | content.alias |
| catid | query | No | integer | content.catid |
| id | path | Yes | integer | content.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /content/{id}/doc

Get Content Doc

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| alias | query | No | string | content.alias |
| catid | query | No | integer | content.catid |
| id | path | Yes | integer | content.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /content

Get Content List

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| categoryIdList | query | No | string | CSV List of category IDs |
| limit | query | No | integer | Limit number of results (Default: 12) |
| offset | query | No | integer | Offset number of results (Default: 0) |
| orderBy | query | No | string | Sort ordering: default (ordering|ASC) |
| q | query | No | string | Query string |
| tagsList | query | No | string | CSV List of tags |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
