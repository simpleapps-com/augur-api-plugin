# Oauth

Datatype for agr_info microservice.

## POST /oauth/refresh

Rotate a refresh token; returns a new access/refresh pair

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /oauth/grants/{grantId}

Revoke a grant; idempotent per RFC 7009 spirit

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| grant_id | path | Yes | string | Grant identifier (UUID) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps (caller) |
| x-target-site-id | header | Yes | string | Target siteId where the grant lives |

---
