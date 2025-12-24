# Code P21

Datatype for p21_core microservice.

## GET /code-p21

List P21 Codes

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| codeNoList | query | No | string | CSV is code_nos to limit results |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | Yes | string | search query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
