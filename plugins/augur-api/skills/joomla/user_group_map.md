# User Group Map

Datatype for joomla microservice.

## GET /users/:id/groups/:groupId

get User Group

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| group_id | path | Yes | integer | usergroups.id |
| id | path | Yes | integer | users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /users/:id/groups

List User Groups

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /users/:id/groups

Create/update User Group Mapping

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | users.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
