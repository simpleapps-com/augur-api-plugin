# Trans Web Display Type

Datatype for p21_apis microservice.

## GET /trans-web-display-type/{webDisplayTypeUid}

Get Web Display Type Details by Display Type UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| webDisplayTypeId | query | No | string | Web Display Type ID |
| web_display_type_uid | path | Yes | integer | Web Display Type UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /trans-web-display-type/{webDisplayTypeUid}

Update Web Display Type by Display Type UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| webDisplayTypeId | query | No | string | Web Display Type ID |
| web_display_type_uid | path | Yes | integer | Web Display Type UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /trans-web-display-type/{webDisplayTypeUid}

Delete Web Display Type by Display Type UID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| webDisplayTypeId | query | No | string | Web Display Type ID |
| web_display_type_uid | path | Yes | integer | Web Display Type UID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /trans-web-display-type/defaults

Get Web Display Type Defaults

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /trans-web-display-type/definition

Get Web Display Type Definition

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /trans-web-display-type

Create Web Display Type

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
