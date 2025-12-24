# Address

Datatype for p21_core microservice.

## GET /address/{id}

Get Address Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| address | path | Yes | integer | address |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /address/{id}/corp-address

Get Corporate Address List

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /address/{id}/default

Set Address as default Shipping Method

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /address/{id}/enable

Enable/disable Address as Shipping Method

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| enabledCd | query | No | int | Shipping Method Enabled Code (enabled_cd) [(704)|705|Blank] |
| id | path | Yes | integer | id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /address/refresh

Trigger a data refresh

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /address

List Addresses

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| carrierFlag | query | No | string | Carrier Flag [(Y)|N|Blank] |
| defaultCd | query | No | int | Shipping Method default Code (default_cd) [704|705|700|Blank] |
| enabledCd | query | No | int | Shipping Method Enabled Code (enabled_cd) [704|705|700|Blank] |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCd | query | No | int | Status Code (status_cd) [(704)|705|700] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
