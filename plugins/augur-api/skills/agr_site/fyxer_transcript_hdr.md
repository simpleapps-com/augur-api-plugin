# Fyxer Transcript Hdr

Datatype for agr_site microservice.

## GET /fyxer-transcript/{fyxerTranscriptHdrUid}

Get Fyxer Transcript Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| fyxer_transcript_hdr_uid | path | Yes | integer | fyxer_transcript_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /fyxer-transcript/{fyxerTranscriptHdrUid}

Update Fyxer Transcript

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| fyxer_transcript_hdr_uid | path | Yes | integer | fyxer_transcript_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /fyxer-transcript/{fyxerTranscriptHdrUid}

DELETE Fyxer Transcript

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| fyxer_transcript_hdr_uid | path | Yes | integer | fyxer_transcript_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /fyxer-transcript

List Fyxer Transcripts

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: fyxer_transcript_hdr_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|(705)|(700)] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /fyxer-transcript

Create Fyxer Transcript

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
