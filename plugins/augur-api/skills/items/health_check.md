# Health Check

Datatype for items microservice.

## GET /health-check

Health Check

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /ping

Ping to get Pong

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /whoami

Whoami

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
