# Todos Summary

Datatype for basecamp2 microservice.

## GET /todos-summary/{id}

Get Todo Summary Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Todo Summary ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /todos-summary

List Todo Summaries

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| akashaCd | query | No | int | Filter by akasha sync status |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| processCd | query | No | int | Filter by process code |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
