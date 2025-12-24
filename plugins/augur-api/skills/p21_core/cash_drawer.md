# Cash Drawer

Datatype for p21_core microservice.

## GET /cash_drawer/{cashDrawerUid}

Get Cash Drawer Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cash_drawer_uid | path | Yes | integer | cash_drawer_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /cash_drawer

List Cash Drawers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | Company ID |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: cash_drawer_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (Default: 704, Options: 704, 705, 700, -1) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
