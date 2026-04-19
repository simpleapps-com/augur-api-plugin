# Context

Datatype for agr_site microservice.

## GET /context/{siteId}

get the context for a site

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| site_id | path | Yes | string | target site ID to get context for |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
