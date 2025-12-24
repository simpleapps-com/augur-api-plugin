# Podcasts

Datatype for p21_pim microservice.

## GET /podcasts/{podcastsUid}

Get Podcast Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| podcasts_uid | path | Yes | integer | podcasts_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /podcasts/{podcastsUid}

Update Podcast

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| podcasts_uid | path | Yes | integer | podcasts_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /podcasts/{podcastsUid}

DELETE Podcast

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| podcasts_uid | path | Yes | integer | podcasts_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /podcasts

List Podcasts

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: podcasts_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /podcasts

Create Podcast

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
