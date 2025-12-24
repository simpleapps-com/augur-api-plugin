# Training Msg

Datatype for agr_site microservice.

## GET /training/{trainingSetUid}/conversations/{trainingConvUid}/messages/{trainingMsgUid}

Get Training Message Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_msg_uid | path | Yes | integer | training_msg_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /training/{trainingSetUid}/conversations/{trainingConvUid}/messages/{trainingMsgUid}

Update Training Message

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_msg_uid | path | Yes | integer | training_msg_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /training/{trainingSetUid}/conversations/{trainingConvUid}/messages/{trainingMsgUid}

DELETE Training Message

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_msg_uid | path | Yes | integer | training_msg_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /training/{trainingSetUid}/conversations/{trainingConvUid}/messages

List Training Messages

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: training_msg_uid|ASC) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /training/{trainingSetUid}/conversations/{trainingConvUid}/messages

Create Training Message

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| training_conv_uid | path | Yes | integer | training_conv_uid |
| training_set_uid | path | Yes | integer | training_set_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
