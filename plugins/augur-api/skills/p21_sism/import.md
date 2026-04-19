# Import

Datatype for p21_sism microservice.

## GET /import/daily-summary

Get daily import counts by state

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| days | query | No | integer | Number of days back from today (Default: 7) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /import/{importUid}

Get the details of an import

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | string | import.import_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /import/{importUid}

Update an import

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | string | import.import_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /import/{importUid}

clean pending_import for an import

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | string | import.import_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /import

Get a list of imports

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| createdFrom | query | No | string | Date range start (YYYY-MM-DD HH:MM:SS). Requires createdTo. |
| createdOn | query | No | string | Filter by single date (YYYY-MM-DD). Returns imports created on that day. |
| createdTo | query | No | string | Date range end (YYYY-MM-DD HH:MM:SS). Requires createdFrom. |
| excludeState | query | No | string | Exclude imports in these states (comma-separated). Ignored if importState is set. |
| importState | query | No | string | Import State filter, comma-separated (Default: initial). Use "all" to disable. |
| limit | query | No | integer | limit number of results (Default: 12) |
| offset | query | No | integer | offset (Default: 0) |
| orderBy | query | No | string | Order By field (Default: import_uid|DESC) |
| q | query | No | string | Search query to filter imports |
| referenceNo | query | No | string | Reference number for direct filtering (often P21 order number, but depends on import type) |
| sourceId | query | No | integer | Filter by source ID |
| sourceName | query | No | string | Filter by source name (e.g. commerce) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /import/recent

Get a list of the most recent imports

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| createdFrom | query | No | string | Date range start (YYYY-MM-DD HH:MM:SS). Requires createdTo. |
| createdOn | query | No | string | Filter by single date (YYYY-MM-DD). Returns imports created on that day. Overrides hours param. |
| createdTo | query | No | string | Date range end (YYYY-MM-DD HH:MM:SS). Requires createdFrom. |
| excludeState | query | No | string | Exclude imports in these states (comma-separated). Ignored if importState is set. |
| hours | query | No | integer | Hours since created (Default: 48) |
| importState | query | No | string | Import State filter, comma-separated. Use "all" to disable. |
| limit | query | No | integer | limit number of results (Default: 1000) |
| sourceId | query | No | integer | Filter by source ID |
| sourceName | query | No | string | Filter by source name (e.g. commerce) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /import/stuck

Get a list of stuck imports

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| hours | query | No | integer | Hours since stuck (Default: 48) |
| limit | query | No | integer | limit number of results (Default: 1000) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
