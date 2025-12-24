# Company

Datatype for p21_core microservice.

## GET /company/{companyUid}

Get Company Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | company_id |
| company_uid | path | Yes | integer | company_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /company

List Companies

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | Company Id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: company_uid|ASC) |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
