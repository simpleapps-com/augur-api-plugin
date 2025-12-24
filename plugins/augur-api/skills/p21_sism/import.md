# Import

Datatype for p21_sism microservice.

## GET /import/{import_uid}

Get the details of an import

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | string | import.import_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /import/{import_uid}

Update an import

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| import_uid | path | Yes | string | import.import_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /import/{import_uid}

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
| importState | query | No | string | Import State [initial|hold|delivered](Default: initial) |
| limit | query | No | integer | limit number of results (Default: 12) |
| offset | query | No | integer | offset (Default: 0) |
| orderBy | query | No | string | Order By field (Default: import_uid|DESC) |
| q | query | No | string | Search query to filter imports |
| referenceNo | query | No | string | Reference number for direct filtering (often P21 order number, but depends on import type) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /import/recent

Get a list of the most recent imports

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| hours | query | No | integer | Hours since created (Default: 48) |
| limit | query | No | integer | limit number of results (Default: 1000) |
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
