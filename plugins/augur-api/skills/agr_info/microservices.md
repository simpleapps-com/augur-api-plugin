# Microservices

Datatype for agr_info microservice.

## GET /microservices/{microservicesUid}

Get Microservice Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| microservices_uid | path | Yes | integer | microservices_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /microservices/{microservicesUid}

Update Microservice

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| microservices_uid | path | Yes | integer | microservices_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /microservices/{microservicesUid}

DELETE Microservice

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| microservices_uid | path | Yes | integer | microservices_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /microservices

List Microservices

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /microservices

Create Microservice

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
