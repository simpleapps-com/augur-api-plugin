# Items

Datatype for p21_pim microservice.

## GET /items/{invMastUid}/suggest-display-desc

Suggest Item Display Description

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| model | query | No | string | LLM to use default: llama3.2-vision:11b |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /items/{invMastUid}/suggest-web-desc

Suggest Item Web Description

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| model | query | No | string | LLM to use default: llama3.2-vision:11b |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
