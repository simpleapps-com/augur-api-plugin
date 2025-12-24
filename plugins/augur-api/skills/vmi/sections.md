# Sections

Datatype for vmi microservice.

## GET /sections/{sectionsUid}

Get section Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| sections_uid | path | Yes | integer | sectionsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /sections/{sectionsUid}

Update section

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| sections_uid | path | Yes | integer | sectionsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /sections/{sectionsUid}

DELETE section

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| sections_uid | path | Yes | integer | sectionsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /sections/{sectionsUid}/enable

Enable/Disable/Delete section

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| sections_uid | path | Yes | integer | sectionsUid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /sections

List sections

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| customerId | query | Yes | integer | Customer Id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCd | query | No | integer | Status Code (status_cd) [(704)|705|700] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /sections

Create section

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
