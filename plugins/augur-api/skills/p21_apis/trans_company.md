# Trans Company

Datatype for p21_apis microservice.

## GET /trans-company/{companyUid}

Get Company Details by Company UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | Company ID |
| company_uid | path | Yes | integer | Company UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /trans-company/{companyUid}

Update Company by Company UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | Company ID |
| company_uid | path | Yes | integer | Company UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /trans-company/{companyUid}

Delete Company by Company UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | Company ID |
| company_uid | path | Yes | integer | Company UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /trans-company

Create Company

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
