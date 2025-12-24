# Contracts Items

Datatype for items microservice.

## GET /contracts/{jobNo}/attributes

list the attributes for contract items

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| job_no | path | Yes | integer | Job number |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /contracts/{jobNo}/items

List contracts items for a job

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| classId5ExcludeList | query | No | string | List of excluded class 5 values (default:blank) |
| classId5List | query | No | string | List of allowed class 5 values (default:blank) |
| displayOnWebFlag | query | No | string | Display on web flag [Y|N|Blank] (Default: Blank) |
| fields | query | No | string | fields to filter with (Default: itemId, itemDesc, ExtendedDesc) |
| filters | query | No | string | A JSON representation of the filters [{attributeUid:attributeValueUid}] |
| includeStock | query | No | string | Include Stock [Y|N] (Default: N) |
| job_no | path | Yes | integer | Job number |
| limit | query | No | int | Limit number of results (Default: 12) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | No | string | search query (optional) |
| sortBy | query | No | string | Field from Document to sort by (Default: item_id) |
| tags | query | No | string | A CSV of tags |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
