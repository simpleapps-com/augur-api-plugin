# Job Price Line

Datatype for pricing microservice.

## GET /job-price-hdr/{jobPriceHdrUid}/lines/{jobPriceLineUid}

Get Job Price Line Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| job_price_hdr_uid | path | Yes | integer | job_price_hdr_uid |
| job_price_line_uid | path | Yes | integer | job_price_line_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /job-price-hdr/{jobPriceHdrUid}/lines

List Job Price Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| invMastUid | query | No | integer | Inventory Master UID |
| job_price_hdr_uid | path | Yes | integer | Job Price Header UID |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: job_price_line_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
