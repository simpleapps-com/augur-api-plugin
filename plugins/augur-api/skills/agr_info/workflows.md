# Workflows

Datatype for agr_info microservice.

## GET /workflows/{workflowsUid}

Get Workflow Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| workflows_uid | path | Yes | integer | workflows_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /workflows/{workflowsUid}

Update Workflow

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| workflows_uid | path | Yes | integer | workflows_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /workflows/{workflowsUid}

Delete Workflow

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| workflows_uid | path | Yes | integer | workflows_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /workflows

List Workflows

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| orderBy | query | No | string | Order By (Default: workflows_uid|ASC) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /workflows

Create Workflow

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
