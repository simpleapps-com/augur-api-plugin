# Suggestions

Datatype for open_search microservice.

## GET /suggestions/{suggestionsUid}

Get Suggestion Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| suggestions_uid | path | Yes | integer | Suggestions UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /suggestions

List Suggestions

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: suggestions_uid|ASC) |
| processCd | query | No | int | Process Code filter |
| query | query | No | string | Search query string |
| queryStringUid | query | No | int | Query String UID filter |
| statusCd | query | No | int | Status Code filter |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /suggestions/suggest

Get search suggestions for autocomplete

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | No | string | Search query string for autocomplete |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
