# Training Conv

Datatype for agr_site microservice.

## GET /training/{trainingSetUid}/conversations/{trainingConvUid}

Get Training Conversation Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /training/{trainingSetUid}/conversations/{trainingConvUid}

Update Training Conversation

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /training/{trainingSetUid}/conversations/{trainingConvUid}

DELETE Training Conversation

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /training/{trainingSetUid}/conversations

List Training Conversations

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: training_conv_uid|ASC) |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /training/{trainingSetUid}/conversations

Create Training Conversation

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
