# Distributors

Datatype for vmi microservice.

## GET /distributors/{distributorsUid}

Get distributor Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributors_uid | path | Yes | integer | distributorsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /distributors/{distributorsUid}

Update distributor

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributors_uid | path | Yes | integer | distributorsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /distributors/{distributorsUid}

DELETE distributor

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributors_uid | path | Yes | integer | distributorsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /distributors/{distributorsUid}/enable

Enable/Disable/Delete distributor

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| distributors_uid | path | Yes | integer | distributorsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /distributors

List distributors

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | integer | Customer Id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCd | query | No | int | Status Code (status_cd) [(704)|705,700] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /distributors

Create distributor

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
