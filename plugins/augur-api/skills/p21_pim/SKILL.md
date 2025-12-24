---
name: P21 Pim API
description: Use when working with health check, inv mast ext, inv mast files, inv mast text, items, podcasts, seed, or making API calls to https://p21-pim.augur-api.com.
version: 1.0.5
---

# P21 Pim

Service-specific knowledge for p21_pim microservice.

## API Documentation

- [OpenAPI Specification](https://p21-pim.augur-api.com/openapi.json)
- [Postman Collection](https://p21-pim.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### inv_mast_ext

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast-ext/{invMastExtUid} | Get Inv Mast Ext Details | [inv_mast_ext.md](inv_mast_ext.md#get-inv-mast-extinvMastExtUid) |
| PUT | /inv-mast-ext/{invMastExtUid} | Update Inv Mast Ext | [inv_mast_ext.md](inv_mast_ext.md#put-inv-mast-extinvMastExtUid) |
| DELETE | /inv-mast-ext/{invMastExtUid} | DELETE Inv Mast Ext | [inv_mast_ext.md](inv_mast_ext.md#delete-inv-mast-extinvMastExtUid) |
| GET | /inv-mast-ext | List Inv Mast Ext | [inv_mast_ext.md](inv_mast_ext.md#get-inv-mast-ext) |
| POST | /inv-mast-ext | Create Inv Mast Ext | [inv_mast_ext.md](inv_mast_ext.md#post-inv-mast-ext) |

### items

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /items/{invMastUid}/suggest-display-desc | Suggest Item Display Description | [items.md](items.md#get-itemsinvMastUidsuggest-display-desc) |
| GET | /items/{invMastUid}/suggest-web-desc | Suggest Item Web Description | [items.md](items.md#get-itemsinvMastUidsuggest-web-desc) |

### podcasts

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /podcasts/{podcastsUid} | Get Podcast Details | [podcasts.md](podcasts.md#get-podcastspodcastsUid) |
| PUT | /podcasts/{podcastsUid} | Update Podcast | [podcasts.md](podcasts.md#put-podcastspodcastsUid) |
| DELETE | /podcasts/{podcastsUid} | DELETE Podcast | [podcasts.md](podcasts.md#delete-podcastspodcastsUid) |
| GET | /podcasts | List Podcasts | [podcasts.md](podcasts.md#get-podcasts) |
| POST | /podcasts | Create Podcast | [podcasts.md](podcasts.md#post-podcasts) |
