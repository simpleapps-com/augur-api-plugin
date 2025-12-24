# Warehouse X Users

Datatype for vmi microservice.

## GET /warehouse/{warehouseUid}/users/{usersId}

Get Warehouse User Assignment

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | User ID from joomla.users |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /warehouse/{warehouseUid}/users/{usersId}

Update Warehouse User Assignment

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | User ID from joomla.users |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /warehouse/{warehouseUid}/users/{usersId}

Remove User from Warehouse (sets status_cd to 700)

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| users_id | path | Yes | integer | User ID from joomla.users |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /warehouse/{warehouseUid}/users

List Warehouses Users

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| statusCdList | query | No | string | CSV of status_cd to filter on [700|704|705] |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /warehouse/{warehouseUid}/users

Create/Update Warehouse User

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| makePrimaryUser | query | No | string | make_primary_user (y|N) |
| warehouse_uid | path | Yes | integer | warehouse_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
