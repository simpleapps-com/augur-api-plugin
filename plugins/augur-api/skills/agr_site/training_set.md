# Training Set

Datatype for agr_site microservice.

## GET /training/{trainingSetUid}

Get Training Set Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /training/{trainingSetUid}

Update Training Set

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /training/{trainingSetUid}

DELETE Training Set

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /training

List Training Sets

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: training_set_uid|ASC) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /training

Create Training Set

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
