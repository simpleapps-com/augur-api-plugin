# Job Price Hdr

Datatype for pricing microservice.

## GET /job-price-hdr/{jobPriceHdrUid}

Get Job Price Header Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| job_price_hdr_uid | path | Yes | integer | job_price_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /job-price-hdr

List Job Price Headers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: job_price_hdr_uid|ASC) |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
