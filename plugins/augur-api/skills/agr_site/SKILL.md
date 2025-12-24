---
name: Agr Site API
description: Use when working with basecamp, basecamp comments, basecamp summary, basecamp threads, basecamp todos, commerce, data type context, fyxer transcript hdr, fyxer transcript line, general, geo codes postal codes, goog mc, health check, items, joomla, legacy, meta files hdr, meta files line, notifications, open search, orders, p21 apis, pricing, profit sharing hdr, profit sharing line, seed, settings, sites, training conv, training msg, training set, vendors, or making API calls to https://agr-site.augur-api.com.
version: 1.0.1
---

# Agr Site

Service-specific knowledge for agr_site microservice.

## API Documentation

- [OpenAPI Specification](https://agr-site.augur-api.com/openapi.json)
- [Postman Collection](https://agr-site.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### fyxer_transcript_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /fyxer-transcript/{fyxerTranscriptHdrUid} | Get Fyxer Transcript Details | [fyxer_transcript_hdr.md](fyxer_transcript_hdr.md#get-fyxer-transcriptfyxerTranscriptHdrUid) |
| PUT | /fyxer-transcript/{fyxerTranscriptHdrUid} | Update Fyxer Transcript | [fyxer_transcript_hdr.md](fyxer_transcript_hdr.md#put-fyxer-transcriptfyxerTranscriptHdrUid) |
| DELETE | /fyxer-transcript/{fyxerTranscriptHdrUid} | DELETE Fyxer Transcript | [fyxer_transcript_hdr.md](fyxer_transcript_hdr.md#delete-fyxer-transcriptfyxerTranscriptHdrUid) |
| GET | /fyxer-transcript | List Fyxer Transcripts | [fyxer_transcript_hdr.md](fyxer_transcript_hdr.md#get-fyxer-transcript) |
| POST | /fyxer-transcript | Create Fyxer Transcript | [fyxer_transcript_hdr.md](fyxer_transcript_hdr.md#post-fyxer-transcript) |

### geo_codes_postal_codes

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /geo-codes-postal-codes/{geoCodesPostalCodesUid} | Get Postal Code Details | [geo_codes_postal_codes.md](geo_codes_postal_codes.md#get-geo-codes-postal-codesgeoCodesPostalCodesUid) |
| GET | /geo-codes-postal-codes | List Postal Codes | [geo_codes_postal_codes.md](geo_codes_postal_codes.md#get-geo-codes-postal-codes) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### meta_files_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /meta-files/robots | Get robots.txt | [meta_files_hdr.md](meta_files_hdr.md#get-meta-filesrobots) |

### notifications

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /notifications | Create Notification | [notifications.md](notifications.md#post-notifications) |

### open_search

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /open-search/embedding | Get Query String Embedding | [open_search.md](open_search.md#get-open-searchembedding) |

### settings

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /settings/{settingsUid} | Get Settings Details | [settings.md](settings.md#get-settingssettingsUid) |
| PUT | /settings/{settingsUid} | Update Settings | [settings.md](settings.md#put-settingssettingsUid) |
| DELETE | /settings/{settingsUid} | DELETE Settings | [settings.md](settings.md#delete-settingssettingsUid) |
| GET | /settings | List Settings | [settings.md](settings.md#get-settings) |
| POST | /settings | Create Settings | [settings.md](settings.md#post-settings) |

### training_conv

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /training/{trainingSetUid}/conversations/{trainingConvUid} | Get Training Conversation Details | [training_conv.md](training_conv.md#get-trainingtrainingSetUidconversationstrainingConvUid) |
| PUT | /training/{trainingSetUid}/conversations/{trainingConvUid} | Update Training Conversation | [training_conv.md](training_conv.md#put-trainingtrainingSetUidconversationstrainingConvUid) |
| DELETE | /training/{trainingSetUid}/conversations/{trainingConvUid} | DELETE Training Conversation | [training_conv.md](training_conv.md#delete-trainingtrainingSetUidconversationstrainingConvUid) |
| GET | /training/{trainingSetUid}/conversations | List Training Conversations | [training_conv.md](training_conv.md#get-trainingtrainingSetUidconversations) |
| POST | /training/{trainingSetUid}/conversations | Create Training Conversation | [training_conv.md](training_conv.md#post-trainingtrainingSetUidconversations) |

### training_msg

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /training/{trainingSetUid}/conversations/{trainingConvUid}/messages/{trainingMsgUid} | Get Training Message Details | [training_msg.md](training_msg.md#get-trainingtrainingSetUidconversationstrainingConvUidmessagestrainingMsgUid) |
| PUT | /training/{trainingSetUid}/conversations/{trainingConvUid}/messages/{trainingMsgUid} | Update Training Message | [training_msg.md](training_msg.md#put-trainingtrainingSetUidconversationstrainingConvUidmessagestrainingMsgUid) |
| DELETE | /training/{trainingSetUid}/conversations/{trainingConvUid}/messages/{trainingMsgUid} | DELETE Training Message | [training_msg.md](training_msg.md#delete-trainingtrainingSetUidconversationstrainingConvUidmessagestrainingMsgUid) |
| GET | /training/{trainingSetUid}/conversations/{trainingConvUid}/messages | List Training Messages | [training_msg.md](training_msg.md#get-trainingtrainingSetUidconversationstrainingConvUidmessages) |
| POST | /training/{trainingSetUid}/conversations/{trainingConvUid}/messages | Create Training Message | [training_msg.md](training_msg.md#post-trainingtrainingSetUidconversationstrainingConvUidmessages) |

### training_set

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /training/{trainingSetUid} | Get Training Set Details | [training_set.md](training_set.md#get-trainingtrainingSetUid) |
| PUT | /training/{trainingSetUid} | Update Training Set | [training_set.md](training_set.md#put-trainingtrainingSetUid) |
| DELETE | /training/{trainingSetUid} | DELETE Training Set | [training_set.md](training_set.md#delete-trainingtrainingSetUid) |
| GET | /training | List Training Sets | [training_set.md](training_set.md#get-training) |
| POST | /training | Create Training Set | [training_set.md](training_set.md#post-training) |
