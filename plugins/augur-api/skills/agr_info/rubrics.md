# Rubrics

Datatype for agr_info microservice.

## GET /rubrics/{rubricsUid}

Get Rubric Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| rubrics_uid | path | Yes | integer | rubrics_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /rubrics/{rubricsUid}

Update Rubric

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| rubrics_uid | path | Yes | integer | rubrics_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /rubrics/{rubricsUid}

Delete Rubric

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| rubrics_uid | path | Yes | integer | rubrics_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /rubrics

List Rubrics

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /rubrics

Create Rubric

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
